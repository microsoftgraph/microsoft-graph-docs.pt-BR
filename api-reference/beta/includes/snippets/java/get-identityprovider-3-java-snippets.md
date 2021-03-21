---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a29d1e17a2c458ef74bf1ac3bda1ca7e0a01acad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960969"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IIdentityProviderCollectionPage identityProviders = graphClient.identityProviders()
    .buildRequest()
    .get();

```