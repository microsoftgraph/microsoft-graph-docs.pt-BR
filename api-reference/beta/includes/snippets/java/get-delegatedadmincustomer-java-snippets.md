---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4af2df58cbc44038358e244594a2fe4860a1659
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202373"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedAdminCustomer delegatedAdminCustomer = graphClient.tenantRelationships().delegatedAdminCustomers("4fdbff88-9d6b-42e0-9713-45c922ba8001")
    .buildRequest()
    .get();

```