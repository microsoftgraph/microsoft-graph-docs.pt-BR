---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eee367596cd74e4283f9c9703b78b1c4c4cd953d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774493"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskTrigger = await graphClient.Print.Printers["{printer-id}"].TaskTriggers["{printTaskTrigger-id}"]
    .Request()
    .GetAsync();

```