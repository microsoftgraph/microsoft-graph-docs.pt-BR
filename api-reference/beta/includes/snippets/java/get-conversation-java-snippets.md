---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96a5fca08f8f317355e00e406aefbee6066edf41
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956871"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Conversation conversation = graphClient.groups("{id}").conversations("{id}")
    .buildRequest()
    .get();

```