---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2527fea596c9cbd79a4829575c8b786558d26cb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879155"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().notebooks("{id}")
    .copyNotebook(groupId,renameAs,notebookFolder,siteCollectionId,siteId)
    .buildRequest()
    .post();

```