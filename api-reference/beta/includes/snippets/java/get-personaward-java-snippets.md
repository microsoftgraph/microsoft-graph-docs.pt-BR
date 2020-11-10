---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd7087f75f2fad30cdbbebb0731ef5e50136cbee
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968383"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAward personAward = graphClient.me().profile().awards("{id}")
    .buildRequest()
    .get();

```