---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0473a1299f3843753e045285f5a654f354f0a4c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970923"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISecurityActionCollectionPage securityActions = graphClient.security().securityActions()
    .buildRequest()
    .get();

```