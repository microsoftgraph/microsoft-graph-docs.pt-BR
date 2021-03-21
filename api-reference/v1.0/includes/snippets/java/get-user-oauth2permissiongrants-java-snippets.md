---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca18a8fc90c6ad0d90f3d8d763e93b4314ada78a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983446"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrantCollectionWithReferencesPage oauth2PermissionGrants = graphClient.users("{id}").oauth2PermissionGrants()
    .buildRequest()
    .get();

```