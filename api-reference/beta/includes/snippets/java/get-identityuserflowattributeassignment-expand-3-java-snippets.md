---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee4d359b8f9bc8ab786dc168b09f372d049922f11426baa21dcb72111d25bc66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900028"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = graphClient.identity().b2cUserFlows("{id}").userAttributeAssignments("{id}")
    .buildRequest()
    .expand("userAttribute")
    .get();

```