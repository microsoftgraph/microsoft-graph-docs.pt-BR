---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb7aba37c21d2c3cb6f9d8ba5b385ff8fd30ce5c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346204"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalogCollectionPage catalogs = graphClient.identityGovernance().entitlementManagement().catalogs()
    .buildRequest()
    .get();

```