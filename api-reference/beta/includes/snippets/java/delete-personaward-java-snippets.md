---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f105faf84fee2539ac6fc8ee7602c8d6702f12a2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971163"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().awards("{personAwardId}")
    .buildRequest()
    .delete();

```