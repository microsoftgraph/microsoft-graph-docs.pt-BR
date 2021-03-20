---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23a9f83bafa390ba356e39839567df5bffd5c915
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969351"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .unsubscribeByMail()
    .buildRequest()
    .post();

```