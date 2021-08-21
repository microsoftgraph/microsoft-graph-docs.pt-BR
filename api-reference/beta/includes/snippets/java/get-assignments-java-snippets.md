---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19c2dcb8010a1a3004bf821c66d12902c1b92df818e054506f6320fad6742bcf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213738"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentCollectionWithReferencesPage assignments = graphClient.privilegedRoles("{id}").assignments()
    .buildRequest()
    .get();

```