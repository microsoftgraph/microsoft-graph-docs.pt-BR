---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 217054885fbcb10c33a568d841ac2339638ae7e6
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870070"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().cloudPC().roleAssignments("id")
    .buildRequest()
    .delete();

```