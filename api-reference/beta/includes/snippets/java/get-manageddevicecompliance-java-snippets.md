---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98a0cf12aa538fa3dceefd115cbb91badefea918
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439943"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagedDeviceCompliance managedDeviceCompliance = graphClient.tenantRelationships().managedTenants().managedDeviceCompliances("{managedDeviceComplianceId}")
    .buildRequest()
    .get();

```