---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3a98a257d6d07e31cce535e1cb912bef3a28cb10
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780820"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteGetApplicableContentTypesForListCollectionPage getApplicableContentTypesForList = graphClient.sites("{siteId}")
    .getApplicableContentTypesForList(SiteGetApplicableContentTypesForListParameterSet
        .newBuilder()
        .withListId("{list-id}")
        .build())
    .buildRequest()
    .get();

```