---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9802e209083ced5294c60e2992b864938bb328ed
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315373"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SamlOrWsFedExternalDomainFederationCollectionPage samlOrWsFedExternalDomainFederation = graphClient.directory().federationConfigurations().graph.samlOrWsFedExternalDomainFederation()
    .buildRequest()
    .filter("domains/any(x: x/id eq 'contoso.com')")
    .get();

```