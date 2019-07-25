---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3290b89c4cf8a2d3d4fdc611c2efd55ada97bbdd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878978"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = graphClient.oAuth2Permissiongrants("{id}")
    .buildRequest()
    .get();

```