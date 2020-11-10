---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51db8742dd9d77a14208f7b2e5a4b1c71d29f32d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972051"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = graphClient.subscriptions("{id}")
    .buildRequest()
    .get();

```