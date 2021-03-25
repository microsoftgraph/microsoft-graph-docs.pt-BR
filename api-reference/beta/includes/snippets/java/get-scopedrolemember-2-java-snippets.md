---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fff22ff72fe871c8a87e3d3a535cda7edd059f17
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210598"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembershipCollectionPage scopedRoleMembers = graphClient.administrativeUnits("{id}").scopedRoleMembers()
    .buildRequest()
    .get();

```