---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf251407a40f8b0dc0cbe206417e82de8d48eb7b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364795"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range("A1:Z10")
    .VisibleView()
    .Range()
    .Request()
    .GetAsync();

```