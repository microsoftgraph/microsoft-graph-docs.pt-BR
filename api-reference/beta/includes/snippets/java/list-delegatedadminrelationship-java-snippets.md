---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0417e6d1bc5b0852b18ef508c29532272d55a8d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210885"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedAdminRelationshipCollectionPage delegatedAdminRelationships = graphClient.tenantRelationships().delegatedAdminRelationships()
    .buildRequest()
    .get();

```