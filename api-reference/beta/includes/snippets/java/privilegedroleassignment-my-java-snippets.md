---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 830b9e07382739002bafc4f71460852ea073ca7444ebab68e30b5526e2f7b16d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099524"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentMyCollectionPage my = graphClient.privilegedRoleAssignments()
    .my()
    .buildRequest()
    .get();

```