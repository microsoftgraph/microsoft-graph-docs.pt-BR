---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6aeaac6be3f11721d48c539279aaf3843098619f7a890a290729d21cb338e73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159387"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementActionCollectionPage managementActions = graphClient.tenantRelationships().managedTenants().managementActions()
    .buildRequest()
    .get();

```