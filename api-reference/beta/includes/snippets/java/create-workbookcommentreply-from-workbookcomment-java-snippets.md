---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36180a9cb23bbf3aa71853febad89469ef7b2dcfa6cba97ea92850e169573679
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217558"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReply workbookCommentReply = new WorkbookCommentReply();
workbookCommentReply.content = "This is my reply to the comment.";
workbookCommentReply.contentType = "plain";

graphClient.drive().items("{id}").workbook().comments("{id}").replies()
    .buildRequest()
    .post(workbookCommentReply);

```