---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5549eba1aecfa25dd654be2fbe9a8aa202dfb54
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971518"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedRoleAssignmentRequestMyCollectionPage my = graphClient.privilegedRoleAssignmentRequests()
    .my()
    .buildRequest()
    .get();

```