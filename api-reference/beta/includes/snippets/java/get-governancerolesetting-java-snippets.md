---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0f96f64379b3db4a67d29d0766a0ed7c4a092d5849f3059c0fbc87cd02a07833
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102425"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleSetting governanceRoleSetting = graphClient.privilegedAccess("azureResources").roleSettings("80dc5d6f-8d89-47b3-953f-01dc909ed3f9")
    .buildRequest()
    .get();

```