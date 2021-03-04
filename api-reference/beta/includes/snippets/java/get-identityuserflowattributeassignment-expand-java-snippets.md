---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33bfa8c5b03284b085750ace3c88b289358ae0bb
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "50435151"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IIdentityUserFlowAttributeAssignmentCollectionPage userAttributeAssignments = graphClient.identity().b2xUserFlows("{id}").userAttributeAssignments()
    .buildRequest()
    .expand("userAttribute")
    .get();

```