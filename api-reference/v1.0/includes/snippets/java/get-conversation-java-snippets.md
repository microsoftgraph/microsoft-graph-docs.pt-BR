---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96a5fca08f8f317355e00e406aefbee6066edf41
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883734"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Conversation conversation = graphClient.groups("{id}").conversations("{id}")
    .buildRequest()
    .get();

```