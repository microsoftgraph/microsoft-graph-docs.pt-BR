---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d82b562d4e046db62cdf972ccb54a482cbcab12
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201821"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserConsentRequestCollectionPage userConsentRequests = graphClient.identityGovernance().appConsent().appConsentRequests("ee245379-e3bb-4944-a997-24115f0b8b5e").userConsentRequests()
    .buildRequest()
    .get();

```