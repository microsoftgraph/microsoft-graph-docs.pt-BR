---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbd9e47f97b35204b840e88d6a09ce0ab7637e5c4a113e7f817935b476bdc125
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375890"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().cloudPC().roleAssignments("id")
    .buildRequest()
    .delete();

```