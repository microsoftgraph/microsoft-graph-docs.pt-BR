---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87cbdd72369a0197c59f4aa1fbac89035f0848761b65df8d5278b38cf5d0762d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900026"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = graphClient.identity().b2cUserFlows("{id}").userAttributeAssignments("{id}")
    .buildRequest()
    .get();

```