---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9237d902a4770b8d8ab0908d01b5dec0ce0b333343c12f55a87263317396422c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156753"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AssignmentOrder assignmentOrder = graphClient.identity().b2cUserFlows("{id}").userAttributeAssignments()
    .getOrder()
    .buildRequest()
    .get();

```