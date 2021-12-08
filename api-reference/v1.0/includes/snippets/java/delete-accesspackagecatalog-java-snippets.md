---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cec175908042357aa1af5f678480a598b782394e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346990"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().catalogs("{accessPackageCatalogId}")
    .buildRequest()
    .delete();

```