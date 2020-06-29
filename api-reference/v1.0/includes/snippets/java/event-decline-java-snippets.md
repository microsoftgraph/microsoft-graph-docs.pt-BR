---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56c99a91ec8dcbcdcf08bd95b44edb98f112ab31
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44900292"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

boolean sendResponse = true;

graphClient.me().events("{id}")
    .decline(comment,sendResponse)
    .buildRequest()
    .post();

```