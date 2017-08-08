# AutoRest Extension Base

Allows to easily create an AutoRest extension.
See https://github.com/olydis/autorest-extension-helloworld for an example of how to reference and use this package - we recommend using that as a starting point!

## Usage

``` JavaScript
import { AutoRestExtension } from "autorest-extension-base";

const extension = new AutoRestExtension();

extension.Add("plugin-name", async autoRestApi => {
  // plugin implementation
  // Available functions:
  // * Information retrieval:
  //       autoRestApi.ListInputs
  //       autoRestApi.ReadFile
  //       autoRestApi.GetValue
  // * Information submission:
  //       autoRestApi.WriteFile
  //       autoRestApi.Message
});

extension.Run();
```
