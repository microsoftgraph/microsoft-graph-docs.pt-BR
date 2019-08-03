---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7141cc6bcc453bee25acb36ebe48a7f6710f6aa
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172983"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IFeatureRolloutPolicyCollectionPage featureRolloutPolicies = graphClient.directory().featureRolloutPolicies()
    .buildRequest()
    .get();

```