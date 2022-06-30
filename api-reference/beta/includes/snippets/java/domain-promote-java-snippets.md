---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80c1b28d133b86eac16df57ea83cb1fb4d6c7cc4
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "66446573"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.domains("contoso.com")
    .promote()
    .buildRequest()
    .post();

```