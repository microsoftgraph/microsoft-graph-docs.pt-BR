---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a40c2493cdc13b3d175e687d4215393ff688b1d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printSettings = new PrintSettings
{
    DocumentConversionEnabled = true
};

var print = new Print();
print.Settings = printSettings;

await graphClient.Print
    .Request()
    .UpdateAsync(print);

```