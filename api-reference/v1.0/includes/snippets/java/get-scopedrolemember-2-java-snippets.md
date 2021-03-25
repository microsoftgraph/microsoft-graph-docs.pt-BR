---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db7e324e93b959d78a2240f1c50049fcd1de4dde
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209989"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembershipCollectionPage scopedRoleMembers = graphClient.directory().administrativeUnits("{id}").scopedRoleMembers()
    .buildRequest()
    .get();

```