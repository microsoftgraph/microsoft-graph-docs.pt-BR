---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2de86a5f6537e9807ca038a814134d33c31cb5f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982905"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UUID keyId = UUID.fromString("f0b0b335-1d71-4883-8f98-567911bfdca6");

String proof = "eyJ0eXAiOiJ...";

graphClient.servicePrincipals("{id}")
    .removeKey(keyId,proof)
    .buildRequest()
    .post();

```