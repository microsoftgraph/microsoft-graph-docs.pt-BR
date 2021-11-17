---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7f426dd1fbf531836552f8c57bf5ed044c6704126d21f89f0d6cdb3ab4158ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272111"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesPublishingProfile onPremisesPublishingProfile = graphClient.onPremisesPublishingProfiles("provisioning")
    .buildRequest()
    .expand("agentGroups")
    .get();

```