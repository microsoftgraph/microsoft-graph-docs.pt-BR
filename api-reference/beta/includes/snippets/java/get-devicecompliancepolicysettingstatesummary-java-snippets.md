---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7cc744d03fbfe0f009357709e17294ab7827e8c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131009"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DeviceCompliancePolicySettingStateSummary deviceCompliancePolicySettingStateSummary = graphClient.tenantRelationships().managedTenants().deviceCompliancePolicySettingStateSummaries("{deviceCompliancePolicySettingStateSummaryId}")
    .buildRequest()
    .get();

```