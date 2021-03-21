---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7341797c2bc620319df03a58d9b5227cb1174bc7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982543"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drives("{drive-id}").items("{item-id}")
    .checkout()
    .buildRequest()
    .post();

```