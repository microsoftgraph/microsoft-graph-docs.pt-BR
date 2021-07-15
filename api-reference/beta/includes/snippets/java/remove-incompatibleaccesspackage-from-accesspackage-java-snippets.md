---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c951bf936557e1b75c174089e3864d48bd5a64bd
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439358"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").incompatibleAccessPackages("{id}").reference()
    .buildRequest()
    .delete();

```