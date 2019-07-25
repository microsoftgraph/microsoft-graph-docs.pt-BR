---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57bee7bbee83d442996bb26b6349e1106522cbc7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855803"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IScopedRoleMembershipCollectionPage scopedRoleMembers = graphClient.administrativeUnits("{id}").scopedRoleMembers()
    .buildRequest()
    .get();

```