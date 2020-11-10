---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94f9cabd325abf05150c165b5f67e5aaee86bc6a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953668"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupLifecyclePolicyCollectionPage groupLifecyclePolicies = graphClient.groupLifecyclePolicies()
    .buildRequest()
    .get();

```