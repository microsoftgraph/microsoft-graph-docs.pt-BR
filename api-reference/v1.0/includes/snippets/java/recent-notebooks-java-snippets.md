---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82497046711fd90da8d458bc5bbd72c540b65ab97e155106946612c69502d0fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57330035"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NotebookGetRecentNotebooksCollectionPage getRecentNotebooks = graphClient.me().onenote().notebooks()
    .getRecentNotebooks(NotebookGetRecentNotebooksParameterSet
        .newBuilder()
        .withIncludePersonalNotebooks(true)
        .build())
    .buildRequest()
    .get();

```