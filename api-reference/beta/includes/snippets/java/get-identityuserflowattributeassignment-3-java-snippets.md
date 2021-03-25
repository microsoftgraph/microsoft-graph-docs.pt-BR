---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d4b43fcb89f96465c6c1961650c577ad04cc4a6
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210732"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = graphClient.identity().b2cUserFlows("{id}").userAttributeAssignments("{id}")
    .buildRequest()
    .get();

```