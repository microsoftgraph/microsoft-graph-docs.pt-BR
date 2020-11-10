---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eea43ccc0b63150c63cb16d5c39f5dc1a1ec3db5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961076"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IIdentityProviderCollectionWithReferencesPage identityProviders = graphClient.identity().b2xUserFlows("{id}").identityProviders()
    .buildRequest()
    .get();

```