---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 020c960b2b5bf5946fb4e0683e49bd89009be571bb560b2f059b1dff5b1ea4c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327393"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReply workbookCommentReply = graphClient.drive().items("{id}").workbook().comments("{id}").replies("{id}")
    .buildRequest()
    .get();

```