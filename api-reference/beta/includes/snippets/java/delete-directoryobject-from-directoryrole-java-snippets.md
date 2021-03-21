---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 552159dacdd917e07876187e18dcc4531566a903
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980418"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryRoles("{id}").members("{id}").reference()
    .buildRequest()
    .delete();

```