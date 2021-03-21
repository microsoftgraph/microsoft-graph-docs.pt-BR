---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a594e245be6dcc4eb2eb6a34059b056a26a5ffd8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980086"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().addresses("{id}")
    .buildRequest()
    .delete();

```