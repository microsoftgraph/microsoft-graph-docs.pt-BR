---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5454e5dc41767c71ebaf963181977b951a7eb370
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967822"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().todo().lists("AAMkADIyAAAhrbPXAAA=")
    .buildRequest()
    .delete();

```