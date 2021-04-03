---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2da6dcacb5e30c9394f84cf3c6277adb76704db6
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507494"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrantCollectionWithReferencesPage oauth2PermissionGrants = graphClient.users("7d54cb02-aaa3-4016-9f9c-a4b49422dd9b").oauth2PermissionGrants()
    .buildRequest()
    .get();

```