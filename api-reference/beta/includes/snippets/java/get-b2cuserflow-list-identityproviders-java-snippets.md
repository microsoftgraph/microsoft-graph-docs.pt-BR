---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae993806b478d21fefc3050cb88ae4343349f7d912a21a225fc8add09ae2cdd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898844"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderCollectionWithReferencesPage identityProviders = graphClient.identity().b2cUserFlows("{id}").identityProviders()
    .buildRequest()
    .get();

```