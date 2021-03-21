---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de8271395ca1edea6f55eab00e7d277b639c7fd6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976143"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicyCollectionWithReferencesPage claimsMappingPolicies = graphClient.servicePrincipals("{id}").claimsMappingPolicies()
    .buildRequest()
    .get();

```