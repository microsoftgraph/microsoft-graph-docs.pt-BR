---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc4de5926c35a25e7ebe73ddd74c96aab982938b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954912"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().events("{id}")
    .buildRequest()
    .delete();

```