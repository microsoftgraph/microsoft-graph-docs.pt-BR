---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68ccfe82a0b93935e3460ab52c4df5e42b196272
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338033"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustomAccessPackageWorkflowExtension customAccessPackageWorkflowExtension = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("32efb28c-9a7a-446c-986b-ca6528c6669d").customAccessPackageWorkflowExtensions("98ffaec5-ae8e-4902-a434-5ffc5d3d3cd0")
    .buildRequest()
    .get();

```