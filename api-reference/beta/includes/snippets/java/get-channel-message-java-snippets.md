---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3528fbff39f2c95c4710155f7b4fa43444bb10e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863411"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.teams("{id}").channels("{id}").messages("{id}")
    .buildRequest()
    .get();

```