---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00e7eed7da64795c534213fbda4d45df5174815a323e7dc70567ac43b08663f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897759"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskDefinition printTaskDefinition = new PrintTaskDefinition();
printTaskDefinition.displayName = "Test TaskDefinitionName";
AppIdentity createdBy = new AppIdentity();
createdBy.displayName = "Requesting App Display Name";
printTaskDefinition.createdBy = createdBy;

graphClient.print().taskDefinitions("{printTaskDefinitionId}")
    .buildRequest()
    .patch(printTaskDefinition);

```