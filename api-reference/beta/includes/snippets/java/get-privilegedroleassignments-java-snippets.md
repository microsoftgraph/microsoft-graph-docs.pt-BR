---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38fdf072b7d41af85f4cd5591ace874f918ee4cb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875724"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "isElevated eq true and expirationDateTime ne null or isElevated eq false"));

IPrivilegedRoleAssignmentCollectionPage privilegedRoleAssignments = graphClient.privilegedRoleAssignments()
    .buildRequest( requestOptions )
    .get();

```