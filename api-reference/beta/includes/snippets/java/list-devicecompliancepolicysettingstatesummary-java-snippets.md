---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9ae51f6af02a6044501012563fc7555f8ed98444bfc054b9f8b64b06db23258
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102112"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content deviceCompliancePolicySettingStateSummary = graphClient.tenantRelationships().managedTenants().deviceCompliancePolicySettingStateSummary()
    .buildRequest()
    .get();

```