---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c45df4499a4711eeeb5498fb8f25bc1e159eace91097a02299615a427dd15977
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102592"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinitionCollectionPage roleDefinitions = graphClient.roleManagement().directory().roleDefinitions()
    .buildRequest()
    .get();

```