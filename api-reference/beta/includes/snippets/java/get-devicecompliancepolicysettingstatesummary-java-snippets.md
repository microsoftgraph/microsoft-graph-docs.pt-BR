---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18b1ed76412b0174b62c737def80c1bb9193b62a430fd28fcbb0d78c593f551a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101719"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content response = graphClient.tenantRelationships().managedTenants().deviceCompliancePolicySettingStateSummarys().{deviceCompliancePolicySettingStateSummaryId}()
    .buildRequest()
    .get();

```