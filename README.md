Download the starter project files as .zip and extract the files to your desktop.

Pro: Git clone to your Xcode projects folder.

## Podfile Configuration
```
post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['CLANG_WARN_DOCUMENTATION_COMMENTS'] = 'NO'
        end
    end
end
```

Copyright © The App Brewery
