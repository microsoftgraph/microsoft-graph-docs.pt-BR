---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31d7db2f8e4dc3f0b6eb0154b3665749d25c9b93
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979540"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().sections("{id}")
    .copyToSectionGroup(id,groupId,renameAs,null,null)
    .buildRequest()
    .post();

```