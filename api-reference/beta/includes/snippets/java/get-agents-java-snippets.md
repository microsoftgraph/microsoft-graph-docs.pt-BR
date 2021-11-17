---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2efbfbab93c807295e1c152fcfe23c9f5ea2ae1bd2da9f791e2525622e8df816
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273283"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesAgentCollectionPage agents = graphClient.onPremisesPublishingProfiles("provisioning").agents()
    .buildRequest()
    .expand("agentGroups")
    .get();

```