---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: beb4b22d92af23999c8d21789693f00925482956
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980213"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITokenLifetimePolicyCollectionPage tokenLifetimePolicies = graphClient.policies().tokenLifetimePolicies()
    .buildRequest()
    .get();

```