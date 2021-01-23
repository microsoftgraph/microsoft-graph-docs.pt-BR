---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54c503f897061ed87496aa8738ec10e42b3f5e7b
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945385"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembership scopedRoleMembership = graphClient.administrativeUnits("{id}").scopedRoleMembers("{id}")
    .buildRequest()
    .get();

```