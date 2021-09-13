---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70c7626fff36791c583ed0770eed30451205ee6c691b69bb9dc58698b071737a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158100"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("microsoftAuthenticator")
    .buildRequest()
    .delete();

```