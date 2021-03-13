---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f382da9918ad373494f88086726a25776e7e700
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808419"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerCapabilities = await graphClient.Print.Printers["{printer-id}"]
    .GetCapabilities()
    .Request()
    .GetAsync();

```