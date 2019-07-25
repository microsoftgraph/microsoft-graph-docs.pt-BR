---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45ccc4d9f4d3ece772223958462705cb022ad81c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880633"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createForward()
    .buildRequest()
    .post();

```