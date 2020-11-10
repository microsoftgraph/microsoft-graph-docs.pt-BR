---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0164d8323c5f23c7dc1f61bc4541c8c576c80887
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956845"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConversationThreadCollectionPage threads = graphClient.groups("{id}").conversations("{id}").threads()
    .buildRequest()
    .get();

```