# AutoRest Extension Base

Allows to easily create an AutoRest extension.

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