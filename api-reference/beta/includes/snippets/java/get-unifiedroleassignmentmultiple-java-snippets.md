---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25264f3f9c48d21b3d23a4be950bf835cd31af66
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179542"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUnifiedRoleAssignmentMultipleCollectionPage roleAssignments = graphClient.roleManagement().deviceManagement().roleAssignments()
    .buildRequest()
    .get();

```