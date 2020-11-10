---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2690546ae7da7d99f0649ca03e4a53511e85909
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957720"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage externalSponsors = graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}").externalSponsors()
    .buildRequest()
    .get();

```