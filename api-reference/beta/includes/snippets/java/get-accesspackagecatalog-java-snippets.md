---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9658ca159941326ec28f53c228da0a5c22766182
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951946"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalog accessPackageCatalog = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("{id}")
    .buildRequest()
    .get();

```