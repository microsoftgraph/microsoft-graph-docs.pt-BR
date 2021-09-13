---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc73a203a499b9c0f95925b3405812bf05723305d28475369f907ceb0974ca5f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327471"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

graphClient.me().onenote().pages("{id}")
    .copyToSection(OnenotePageCopyToSectionParameterSet
        .newBuilder()
        .withId(id)
        .withGroupId(groupId)
        .withSiteCollectionId(null)
        .withSiteId(null)
        .build())
    .buildRequest()
    .post();

```