---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09766d9b33f83221bffcc28ea1df0203f7f4dcd8
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208874"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignmentCollectionPage userAttributeAssignments = graphClient.identity().b2xUserFlows("{id}").userAttributeAssignments()
    .buildRequest()
    .expand("userAttribute")
    .get();

```