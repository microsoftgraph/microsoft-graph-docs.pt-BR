---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a511741334c8ea783ae011c84cc6904697ad9eadce76f99484a24f086cde1ee3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272289"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceEndpoint printServiceEndpoint = graphClient.print().services("{id}").endpoints("{name}")
    .buildRequest()
    .get();

```