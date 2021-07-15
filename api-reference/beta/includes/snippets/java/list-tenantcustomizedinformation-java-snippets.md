---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad2e3bd4f593bb79d87505ced7afb73dadd3870e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440628"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantCustomizedInformationCollectionPage tenantsCustomizedInformation = graphClient.tenantRelationships().managedTenants().tenantsCustomizedInformation()
    .buildRequest()
    .get();

```