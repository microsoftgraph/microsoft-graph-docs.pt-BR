---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59ad9ce97bde852928fbc771b9c3da48ba9ff0f1be197a1cb01c6d3b71b5b90a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101969"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRole privilegedRole = graphClient.privilegedRoles("{id}")
    .buildRequest()
    .get();

```