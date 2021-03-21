---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb0de301d5c17dc1b437fab81d486eec6b178e59
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975897"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.oauth2PermissionGrants("{id}")
    .buildRequest()
    .delete();

```