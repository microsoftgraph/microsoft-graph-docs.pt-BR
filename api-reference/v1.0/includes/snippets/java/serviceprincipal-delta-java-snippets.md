---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8683e0f7ef0cf356ca9067e986c89f3503a77683
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46569997"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IServicePrincipalDeltaCollectionPage delta = graphClient.servicePrincipals()
    .delta()
    .buildRequest()
    .get();

```