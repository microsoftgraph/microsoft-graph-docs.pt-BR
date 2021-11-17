---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9b4fec152899634790a5ce0914c2dded904eebdb84468dda1b96f5225cda4dc7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328043"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WindowsProtectionState windowsProtectionState = graphClient.tenantRelationships().managedTenants().windowsProtectionStates("{windowsProtectionStateId}")
    .buildRequest()
    .get();

```