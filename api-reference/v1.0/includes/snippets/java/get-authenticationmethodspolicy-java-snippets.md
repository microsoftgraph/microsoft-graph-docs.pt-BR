---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 225c6663a73282cd0c166cf3c76ccd212e52813fa994cfb353645974b2f9ec93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100686"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethodsPolicy authenticationMethodsPolicy = graphClient.policies().authenticationMethodsPolicy()
    .buildRequest()
    .get();

```