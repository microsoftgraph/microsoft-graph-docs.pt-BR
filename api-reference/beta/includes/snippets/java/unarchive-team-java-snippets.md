---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1966cb16fe66a390685fcb46acd0bca3dc6ccc2d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978716"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}")
    .unarchive()
    .buildRequest()
    .post();

```