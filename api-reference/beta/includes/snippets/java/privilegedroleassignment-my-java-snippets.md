---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30796950cc49a36f7a1cb5b26d61bba7ba29f798
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980595"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentMyCollectionPage my = graphClient.privilegedRoleAssignments()
    .my()
    .buildRequest()
    .get();

```