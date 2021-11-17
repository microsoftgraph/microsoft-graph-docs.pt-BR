---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21593c247a6112ab7d9892c9e6a32ecccf776f4df5ad7dbe1b5e7c2dea266972
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214640"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcConnectionCollectionPage cloudPcConnections = graphClient.tenantRelationships().managedTenants().cloudPcConnections()
    .buildRequest()
    .get();

```