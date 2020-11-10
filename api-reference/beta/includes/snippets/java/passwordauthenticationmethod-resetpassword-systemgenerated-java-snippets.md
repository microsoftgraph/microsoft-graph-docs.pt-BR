---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19fad558e8d8aaa7d2b18b7d87729645b55ec184
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968677"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id | userPrincipalName}").authentication().passwordMethods("{id}")
    .resetPassword(null,null)
    .buildRequest()
    .post();

```