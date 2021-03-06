# appcode-live-templates

Collection of live templates for AppCode

## Installation

1. Clone this repository
1. Copy Objective-C.xml file to ```~/Library/Preferences/AppCode<version>/templates```
1. Restart AppCode.

## Templates

### propn

Insert nonatomic property

```
@property(nonatomic) $DECLARATION$;$END$
```

### propnro

Insert nonatomic read only property.

```
@property(nonatomic, readonly) $DECLARATION$;$END$
```

### propns

Insert nonatomic strong property.
```
@property(nonatomic, strong) $DECLARATION$;$END$
```

### privcat

Insert private category code block.
```
@interface $CLASS_NAME$ ()
$END$
@end
```

### wself

Insert weakSelf statement, i.e. weak reference to self.
```
__weak typeof(self) weakSelf = self;
```

### wselfs

Insert strong reference to weakSelf. Useful in pair with wself template
```
__strong __auto_type strongSelf = weakSelf;
```

### propnw

Insert nonatomic weak property.
```
@property(nonatomic, weak) $DECLARATION$;$END$
```

### propnwo

Insert nonatomic weak IBOutlet property.
```
@property(nonatomic, weak) IBOutlet $DECLARATION$;$END$
```

### ncadd

Add NSNotificationCenter observer
```
[[NSNotificationCenter defaultCenter] addObserver:$OBS$
                                selector:@selector($SELECTOR$)
                                name:$NAME$
                                object:$OBJ$];$END$
```

### dafter

Dispatch after in Main queue
```
dispatch_after(dispatch_time(DISPATCH_TIME_NOW, (int64_t)($TIME$ * NSEC_PER_SEC)), dispatch_get_main_queue(), ^{
    $CODE$
});
```
