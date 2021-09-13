---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f78421e1a2db4b1c9a8ec7f2f03745a1c6c05ace39e2e46fcc4e9bd571454cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900055"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkforceIntegration workforceIntegration = graphClient.teamwork().workforceIntegrations("{workforceintegrationid}")
    .buildRequest()
    .get();

```