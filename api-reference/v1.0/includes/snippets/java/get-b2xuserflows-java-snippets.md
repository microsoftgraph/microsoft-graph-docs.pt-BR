---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4e1a681ff3379a161c133f3602aeab8ebd062d538e0ab5bbc9840ca9ff8e1b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216120"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2xIdentityUserFlow b2xIdentityUserFlow = graphClient.identity().b2xUserFlows("B2X_1_PartnerSignUp")
    .buildRequest()
    .get();

```