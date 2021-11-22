---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 848377ba754eaaefc218e6d57b63223be4e99bdd51cf10a3d77d1cc36dd8b63b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326988"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOverview cloudPcOverview = graphClient.tenantRelationships().managedTenants().cloudPcsOverview("{cloudPcOverviewId}")
    .buildRequest()
    .get();

```