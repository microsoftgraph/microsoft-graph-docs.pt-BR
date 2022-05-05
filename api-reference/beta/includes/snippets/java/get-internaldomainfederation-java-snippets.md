---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 291880059b8355c5a60ee9c6287832cba80be737
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212156"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InternalDomainFederation internalDomainFederation = graphClient.domains("contoso.com").federationConfiguration("6601d14b-d113-8f64-fda2-9b5ddda18ecc")
    .buildRequest()
    .get();

```