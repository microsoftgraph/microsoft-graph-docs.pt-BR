---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed2ceec86e2dae071fcc51dacffbe1fb888b56a2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983543"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOAuth2PermissionGrantCollectionWithReferencesPage oauth2PermissionGrants = graphClient.servicePrincipals("{id}").oauth2PermissionGrants()
    .buildRequest()
    .get();

```