---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d82b562d4e046db62cdf972ccb54a482cbcab12
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507376"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserConsentRequestCollectionPage userConsentRequests = graphClient.identityGovernance().appConsent().appConsentRequests("ee245379-e3bb-4944-a997-24115f0b8b5e").userConsentRequests()
    .buildRequest()
    .get();

```