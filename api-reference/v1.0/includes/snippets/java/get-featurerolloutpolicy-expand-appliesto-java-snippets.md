---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89aeaddcec762324d84889261d221860fceff108
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201384"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FeatureRolloutPolicy featureRolloutPolicy = graphClient.directory().featureRolloutPolicies("df85e4d9-e8c4-4033-a41c-73419a95c29c")
    .buildRequest()
    .expand("appliesTo")
    .get();

```