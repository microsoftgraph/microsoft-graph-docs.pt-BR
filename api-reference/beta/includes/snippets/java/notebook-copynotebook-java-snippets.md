---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8e7cb10e540c304087bd7b881d4ded3f8eb7246e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983379"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().notebooks("{id}")
    .copyNotebook(NotebookCopyNotebookParameterSet
        .newBuilder()
        .withGroupId(groupId)
        .withRenameAs(renameAs)
        .withNotebookFolder(null)
        .withSiteCollectionId(null)
        .withSiteId(null)
        .build())
    .buildRequest()
    .post();

```