---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 645d281ef47479f4921a97515e7b2f2227f5a8e1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969537"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubscribedSku subscribedSku = graphClient.subscribedSkus("{id}")
    .buildRequest()
    .get();

```