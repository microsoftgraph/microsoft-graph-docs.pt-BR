---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0276056755837eb71f3b983f4287224039d78ee0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337949"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustomAccessPackageWorkflowExtensionCollectionPage customAccessPackageWorkflowExtensions = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("32efb28c-9a7a-446c-986b-ca6528c6669d").customAccessPackageWorkflowExtensions()
    .buildRequest()
    .get();

```