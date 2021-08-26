---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44df4938cf21b68c23bda537760d2adad5fc429fedac521698c9cbeff6149bfa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102240"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteGetApplicableContentTypesForListCollectionPage getApplicableContentTypesForList = graphClient.sites("{siteId}")
    .getApplicableContentTypesForList(SiteGetApplicableContentTypesForListParameterSet
        .newBuilder()
        .withListId("listId")
        .build())
    .buildRequest()
    .get();

```