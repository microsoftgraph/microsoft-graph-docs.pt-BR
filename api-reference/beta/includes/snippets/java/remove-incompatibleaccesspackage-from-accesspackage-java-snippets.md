---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad6ebea25b627be2b54282baea5ab36eed60aa4913ad2c50cad72585938c8a77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099911"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").incompatibleAccessPackages("{id}").reference()
    .buildRequest()
    .delete();

```