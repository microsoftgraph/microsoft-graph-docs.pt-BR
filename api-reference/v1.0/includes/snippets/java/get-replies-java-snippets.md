---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69486895596376a59b2e368f1f70601ea73447eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980864"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReplyCollectionPage replies = graphClient.drive().items("{id}").workbook().comments("{id}").replies()
    .buildRequest()
    .get();

```