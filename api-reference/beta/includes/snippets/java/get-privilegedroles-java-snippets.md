---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 802c666ca6f2d8e64595318d843d34c8cb1fa2f9da906fbf0ff89c8ad074a0a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272663"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleCollectionPage privilegedRoles = graphClient.privilegedRoles()
    .buildRequest()
    .get();

```