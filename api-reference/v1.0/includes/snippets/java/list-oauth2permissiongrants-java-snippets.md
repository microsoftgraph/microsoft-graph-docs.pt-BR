---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af89914b72814d21a91d3740df539cc091ed9483
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335293"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOAuth2PermissionGrantCollectionPage oauth2PermissionGrants = graphClient.oauth2PermissionGrants()
    .buildRequest()
    .get();

```