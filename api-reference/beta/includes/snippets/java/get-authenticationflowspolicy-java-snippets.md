---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09a5c9e8e357ca293492e2dd5f5253ae0a96352427c0199f267d56820a8d7b89
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100176"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationFlowsPolicy authenticationFlowsPolicy = graphClient.policies().authenticationFlowsPolicy()
    .buildRequest()
    .get();

```