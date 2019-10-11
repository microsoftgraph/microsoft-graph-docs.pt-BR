---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce4cb8a5c210e1ba37e4990499af5d3298fef7b8
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428760"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createReply(null,null)
    .buildRequest()
    .post();

```