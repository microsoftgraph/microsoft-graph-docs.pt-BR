---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6721080394fcb0652d9772d029241938e368efdf4d2e9ccdffa704218210c41c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899882"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FeatureRolloutPolicyCollectionPage featureRolloutPolicies = graphClient.policies().featureRolloutPolicies()
    .buildRequest()
    .get();

```