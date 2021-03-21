---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32042ebaa75f0e7ff3af6ef8df368ca88ec4702b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972831"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{id}")
    .buildRequest()
    .delete();

```