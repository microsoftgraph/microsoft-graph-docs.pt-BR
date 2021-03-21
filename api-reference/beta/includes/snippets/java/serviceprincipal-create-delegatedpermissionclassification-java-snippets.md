---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d944acc26d93ebea0628cd56eb224a7f67c6048
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981342"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedPermissionClassification delegatedPermissionClassification = new DelegatedPermissionClassification();
delegatedPermissionClassification.permissionId = "e1fe6dd8-ba31-4d61-89e7-88639da4683d";
delegatedPermissionClassification.permissionName = "User.Read";
delegatedPermissionClassification.classification = PermissionClassificationType.LOW;

graphClient.servicePrincipals("{id}").delegatedPermissionClassifications()
    .buildRequest()
    .post(delegatedPermissionClassification);

```