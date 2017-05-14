# appcode-live-templates

Collection of live templates for AppCode

## Installation

1. Clone this repository
1. Copy Objective-C.xml file to ```~/Library/Preferences/AppCode<version>/templates``` 
1. Restart AppCode.

## Templates

### propnro

Insert nonatomic weak property.

```
@property(nonatomic, weak) $DECLARATION$;$END$
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

Insert weak reference to self.
```
__weak typeof(self) weakSelf = self;
```

### propnw

Insert nonatomic weak property.
```
@property(nonatomic, weak) $DECLARATION$;$END$
```