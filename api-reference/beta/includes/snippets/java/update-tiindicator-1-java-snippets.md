---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61bbf3f51769ad7fee943cc9d324238e732d9dc1c0f88756d5a69d910b0698e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216273"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TiIndicator tiIndicator = new TiIndicator();
tiIndicator.description = "description-updated";

graphClient.security().tiIndicators("{id}")
    .buildRequest()
    .patch(tiIndicator);

```