---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: faa4ce57825840aa82414a9ca18a68fe8d013356bc10930176809f15c259eeb2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213877"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignmentCollectionPage userAttributeAssignments = graphClient.identity().b2cUserFlows("{id}").userAttributeAssignments()
    .buildRequest()
    .get();

```