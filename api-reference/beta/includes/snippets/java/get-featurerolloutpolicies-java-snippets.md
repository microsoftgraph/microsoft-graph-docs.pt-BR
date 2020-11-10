---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7141cc6bcc453bee25acb36ebe48a7f6710f6aa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963259"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IFeatureRolloutPolicyCollectionPage featureRolloutPolicies = graphClient.directory().featureRolloutPolicies()
    .buildRequest()
    .get();

```