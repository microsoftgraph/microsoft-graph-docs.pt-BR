---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d54f072907f09fee10aace6e789390fa9fba73a3
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519604"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalog accessPackageCatalog = new AccessPackageCatalog();
accessPackageCatalog.displayName = "Catalog One";

graphClient.identityGovernance().entitlementManagement().catalogs("{accessPackageCatalogId}")
    .buildRequest()
    .patch(accessPackageCatalog);

```