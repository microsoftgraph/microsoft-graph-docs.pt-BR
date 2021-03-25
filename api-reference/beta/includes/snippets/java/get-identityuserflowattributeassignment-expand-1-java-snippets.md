---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acc061a0f554d5797867cd1396abd4dd3af177a2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211164"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignmentCollectionPage userAttributeAssignments = graphClient.identity().b2cUserFlows("{id}").userAttributeAssignments()
    .buildRequest()
    .expand("userAttribute")
    .get();

```