---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 305360a3a68409d5af3f22418fd2042a087db016fe5b2bce423c104cc3788d79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215571"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesAgentGroup onPremisesAgentGroup = graphClient.onPremisesPublishingProfiles("provisioning").agentGroups("2d55ed41-1619-4848-92bb-0576d3038682")
    .buildRequest()
    .expand("agents")
    .get();

```