---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3a61c82e8730352eeee5fa5a803ff9ff7fe3fae8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870012"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOAuth2PermissionGrantCollectionPage oauth2PermissionGrants = graphClient.servicePrincipals("{id}").oauth2PermissionGrants()
    .buildRequest()
    .get();

```