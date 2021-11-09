---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48dc226343df9b6fbdacb4ca39faffdb9f948fbf
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60736632"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookCommentReply = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Comments["{workbookComment-id}"].Replies["{workbookCommentReply-id}"]
    .Request()
    .GetAsync();

```