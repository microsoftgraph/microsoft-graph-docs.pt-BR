---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5091c8ee9e313a06f6b67da01c75b74cd7a2aadb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967222"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").acceptedSenders().references()
    .buildRequest()
    .delete();

```