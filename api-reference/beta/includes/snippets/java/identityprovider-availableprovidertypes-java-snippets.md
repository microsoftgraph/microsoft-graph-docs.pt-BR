---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 223272a81f191dbd5a2194cfaec40fa537cd26cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971338"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderAvailableProviderTypesCollectionPage availableProviderTypes = graphClient.identityProviders()
    .availableProviderTypes()
    .buildRequest()
    .get();

```