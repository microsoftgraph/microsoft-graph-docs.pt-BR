---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8f07cbfc8e9bdbf7a4233c7c908c0c4502cd4c85acae029e8755e2bfdb441b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898820"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = graphClient.identityGovernance().entitlementManagement().accessPackages("{id}")
    .buildRequest()
    .expand("accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)")
    .get();

```