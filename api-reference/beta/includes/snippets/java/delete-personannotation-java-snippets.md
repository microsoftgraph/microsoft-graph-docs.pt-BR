---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ff8d35ad16389047f1230d3896a4748c8f47fe9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980426"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().notes("{id}")
    .buildRequest()
    .delete();

```