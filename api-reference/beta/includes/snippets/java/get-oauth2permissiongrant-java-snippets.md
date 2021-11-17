---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97645dfc20f1096d8e961ccbeea930de35e38385
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032316"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = graphClient.oauth2PermissionGrants("AVs6JuUDjkCFV7q2gd8QTPimBBgj5iBFj0C6GwwRxC0")
    .buildRequest()
    .get();

```