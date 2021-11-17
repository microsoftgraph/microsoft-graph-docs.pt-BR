---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a74f3adf4c9bf7d95b9871d613e6eeab41ff7de47ff2bdcea21acd190f1e23a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272320"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagedDeviceComplianceTrend managedDeviceComplianceTrend = graphClient.tenantRelationships().managedTenants().managedDeviceComplianceTrends("{managedDeviceComplianceTrendId}")
    .buildRequest()
    .get();

```