---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03f0f89388463d13172bfbfe5e8bbe7b341a67c7c0264a90f5d78d99a84d4e51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100874"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRoleTemplate directoryRoleTemplate = graphClient.directoryRoleTemplates("{id}")
    .buildRequest()
    .get();

```