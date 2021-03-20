---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54c503f897061ed87496aa8738ec10e42b3f5e7b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943000"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembership scopedRoleMembership = graphClient.administrativeUnits("{id}").scopedRoleMembers("{id}")
    .buildRequest()
    .get();

```