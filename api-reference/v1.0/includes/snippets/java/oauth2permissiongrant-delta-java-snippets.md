---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac1139c89ed87ac37b53850bd01f20fe8515d99a
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570018"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOAuth2PermissionGrantDeltaCollectionPage delta = graphClient.oauth2permissiongrants()
    .delta()
    .buildRequest()
    .get();

```