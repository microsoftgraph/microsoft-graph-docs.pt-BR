---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c49890ccf4812ed88963c954c9c21ec3c55b48a8
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474083"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignIn signIn = graphClient.auditLogs().signIns("66ea54eb-blah-4ee5-be62-ff5a759b0100")
    .buildRequest()
    .get();

```