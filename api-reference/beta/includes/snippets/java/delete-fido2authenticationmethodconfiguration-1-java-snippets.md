---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c106d1556ce5fbf198569a8d47cc1a670bb7b3ed8d17b6e0c7a25823cc632c2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272121"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("fido2")
    .buildRequest()
    .delete();

```