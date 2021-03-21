---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 199991d652531c3c1351c0d792a3c0ea487b8f40
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969781"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.devices("{id}").registeredOwners("{id}").reference()
    .buildRequest()
    .delete();

```