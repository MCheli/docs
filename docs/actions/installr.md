<!--
This file is auto-generated and will be re-generated every time the docs are updated.
To modify it, go to its source at https://github.com/fastlane/fastlane/blob/master/fastlane/lib/fastlane/actions/installr.rb
-->

# installr


Upload a new build to [Installr](http://installrapp.com/)







installr ||
---|---
Supported platforms | ios
Author | @scottrhoyt



## 1 Example

```ruby
installr(
  api_token: "...",
  ipa: "test.ipa",
  notes: "The next great version of the app!",
  notify: "dev,qa",
  add: "exec,ops"
)
```





## Parameters

Key | Description | Default
----|-------------|--------
  `api_token` | API Token for Installr Access | 
  `ipa` | Path to your IPA file. Optional if you use the _gym_ or _xcodebuild_ action | [*](#parameters-legend-dynamic)
  `notes` | Release notes | 
  `notify` | Groups to notify (e.g. 'dev,qa') | 
  `add` | Groups to add (e.g. 'exec,ops') | 

<em id="parameters-legend-dynamic">* = default value is dependent on the user's system</em>


<hr />



## Lane Variables

Actions can communicate with each other using a shared hash `lane_context`, that can be accessed in other actions, plugins or your lanes: `lane_context[SharedValues:XYZ]`. The `installr` action generates the following Lane Variables:

SharedValue | Description 
------------|-------------
  `SharedValues::INSTALLR_BUILD_INFORMATION` | Contains release info like :appData. See http://help.installrapp.com/api/

To get more information check the [Lanes documentation](https://docs.fastlane.tools/advanced/lanes/#lane-context).
<hr />


## Documentation

To show the documentation in your terminal, run
```no-highlight
fastlane action installr
```

<hr />

## CLI

It is recommended to add the above action into your `Fastfile`, however sometimes you might want to run one-offs. To do so, you can run the following command from your terminal

```no-highlight
fastlane run installr
```

To pass parameters, make use of the `:` symbol, for example

```no-highlight
fastlane run installr parameter1:"value1" parameter2:"value2"
```

It's important to note that the CLI supports primitive types like integers, floats, booleans, and strings. Arrays can be passed as a comma delimited string (e.g. `param:"1,2,3"`). Hashes are not currently supported.

It is recommended to add all _fastlane_ actions you use to your `Fastfile`.

<hr />

## Source code

This action, just like the rest of _fastlane_, is fully open source, <a href="https://github.com/fastlane/fastlane/blob/master/fastlane/lib/fastlane/actions/installr.rb" target="_blank">view the source code on GitHub</a>

<hr />

<a href="/actions/"><b>Back to actions</b></a>
