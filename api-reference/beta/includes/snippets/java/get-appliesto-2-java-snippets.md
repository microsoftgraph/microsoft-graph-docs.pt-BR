---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5764e055323bc7386d029f4a6b4ee3a9bfb5657
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208569"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().homeRealmDiscoveryPolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```