---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 388affeaa6efd217cb8a0662d3fddc989aa2e5573a985251b39b76c94785a156
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099897"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCollectionWithReferencesPage accessPackagesIncompatibleWith = graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").accessPackagesIncompatibleWith()
    .buildRequest()
    .get();

```