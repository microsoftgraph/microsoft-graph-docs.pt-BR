---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7694a5f7ef72c61482d2927a2f1746f5506b3d4e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803388"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookCommentReply = await graphClient.Drive.Items["{driveItem-id}"].Workbook.Comments["{workbookComment-id}"].Replies["{workbookCommentReply-id}"]
    .Request()
    .GetAsync();

```