---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f770cf7f040a3320fb5d9b999a4b2398a633b33a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979170"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRiskyUserCollectionPage riskyUsers = graphClient.identityProtection().riskyUsers()
    .buildRequest()
    .filter("riskLevel eq microsoft.graph.riskLevel'medium'")
    .get();

```