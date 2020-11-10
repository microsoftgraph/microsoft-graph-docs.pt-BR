---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04f2e0ba9d12e23783813ef661f19c44f4122e98
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973142"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SkillProficiency skillProficiency = graphClient.me().profile().skills("{id}")
    .buildRequest()
    .get();

```