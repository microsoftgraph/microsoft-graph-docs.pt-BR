---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1590d62ec112b0453571d48852741ca6a502380
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439408"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").incompatibleGroups("{id}").reference()
    .buildRequest()
    .delete();

```