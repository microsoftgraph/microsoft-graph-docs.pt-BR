---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4817493af5672f61182092c9b22adf3613b08240
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351607"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().homeRealmDiscoveryPolicies("6c6f154f-cb39-4ff9-bf5b-62d5ad585cde").appliesTo()
    .buildRequest()
    .get();

```