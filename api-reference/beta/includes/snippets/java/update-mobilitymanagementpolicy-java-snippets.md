---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95e7fa12f25c8fbb1f10a38d2a409316452bc2ed
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368793"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MobilityManagementPolicy mobilityManagementPolicy = new MobilityManagementPolicy();
mobilityManagementPolicy.complianceUrl = "https://portal.mg.contoso.com/?portalAction=Compliance";
mobilityManagementPolicy.discoveryUrl = "https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc";
mobilityManagementPolicy.termsOfUseUrl = "https://portal.mg.contoso.com/TermsofUse.aspx";

graphClient.policies().mobileAppManagementPolicies("ab90bacf-55a3-4a3e-839a-aa4b74e4f020")
    .buildRequest()
    .patch(mobilityManagementPolicy);

```