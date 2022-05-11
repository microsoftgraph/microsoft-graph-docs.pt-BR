---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c49a1e21f26fb8e3b231fd49b7f320a9e2d60d97
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315243"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SamlOrWsFedExternalDomainFederation samlOrWsFedExternalDomainFederation = new SamlOrWsFedExternalDomainFederation();
samlOrWsFedExternalDomainFederation.displayName = "Contoso name change";
samlOrWsFedExternalDomainFederation.issuerUri = "http://contoso-test.com/adfs/services/trust";
samlOrWsFedExternalDomainFederation.metadataExchangeUri = null;
samlOrWsFedExternalDomainFederation.signingCertificate = "M66C6DCCAdCgAwIBAgIQQ6vYJIVKQ";
samlOrWsFedExternalDomainFederation.passiveSignInUri = "https://contoso-test.com/adfs/ls/";
samlOrWsFedExternalDomainFederation.preferredAuthenticationProtocol = AuthenticationProtocol.WS_FED;

graphClient.directory().federationConfigurations().graph.samlOrWsFedExternalDomainFederation("d5a56845-6845-d5a5-4568-a5d54568a5d5")
    .buildRequest()
    .patch(samlOrWsFedExternalDomainFederation);

```