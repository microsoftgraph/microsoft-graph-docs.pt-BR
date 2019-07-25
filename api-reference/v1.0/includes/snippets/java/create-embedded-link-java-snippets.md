---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 497ae67c34b9058605129acbfcbfe74842cc4a99
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881816"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "embed";

graphClient.me().drive().items("{item-id}")
    .createLink(type,scope)
    .buildRequest()
    .post();

```