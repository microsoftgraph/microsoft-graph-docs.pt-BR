---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dad0a5f9b0c2638c7b561edf8f7e754057011a69
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441202"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WindowsProtectionState windowsProtectionState = graphClient.tenantRelationships().managedTenants().windowsProtectionStates("{windowsProtectionStateId}")
    .buildRequest()
    .get();

```