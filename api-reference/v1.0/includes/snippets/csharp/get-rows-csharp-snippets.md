---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6182349af1144858079cee74cb61794ef728ac35
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36307734"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range("A1:Z10")
    .VisibleView().Rows
    .Request()
    .GetAsync();

```