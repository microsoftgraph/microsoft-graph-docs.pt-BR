---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c225ab52bea01f81d275b70228850fbe78654ead
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44900329"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

boolean sendResponse = true;

graphClient.me().events("{id}")
    .tentativelyAccept(comment,sendResponse)
    .buildRequest()
    .post();

```