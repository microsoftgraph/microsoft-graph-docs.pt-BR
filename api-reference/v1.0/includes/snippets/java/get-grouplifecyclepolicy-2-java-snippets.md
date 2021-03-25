---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70ab5c695fa323a0242566bf7907a501d09b4684
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210273"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupLifecyclePolicyCollectionPage groupLifecyclePolicies = graphClient.groupLifecyclePolicies()
    .buildRequest()
    .get();

```