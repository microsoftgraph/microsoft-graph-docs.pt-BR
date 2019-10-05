---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a332e99d6bf9de7b88f3dc9de1a30553c37982dd
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402814"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "embed";

graphClient.me().drive().items("{item-id}")
    .createLink(type,null)
    .buildRequest()
    .post();

```