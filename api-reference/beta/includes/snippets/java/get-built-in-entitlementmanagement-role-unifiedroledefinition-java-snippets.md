---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2baf09a9df5d85fac1a75029da11b7ac722e51c6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440698"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinition unifiedRoleDefinition = graphClient.roleManagement().entitlementManagement().roleDefinitions("ba92d953-d8e0-4e39-a797-0cbedb0a89e8")
    .buildRequest()
    .get();

```