---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7912d99a33748fff5dfa51479b65871a62f10913
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41497334"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReply workbookCommentReply = new WorkbookCommentReply();
workbookCommentReply.content = "This is my reply to the comment.";
workbookCommentReply.contentType = "plain";

graphClient.drive().items("{id}").workbook().comments("{id}").replies()
    .buildRequest()
    .post(workbookCommentReply);

```