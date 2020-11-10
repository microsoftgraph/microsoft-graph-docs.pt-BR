---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0155a4b825a9d4c09cb145d326d64d66e3e9cd9e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955038"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EntitlementManagementSettings entitlementManagementSettings = graphClient.identityGovernance().entitlementManagement().settings()
    .buildRequest()
    .get();

```