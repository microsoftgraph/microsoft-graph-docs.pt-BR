---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3a694188ba1b3ccf7d6c3861723e8503e4d6768
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982244"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.devices("{id}")
    .buildRequest()
    .delete();

```