---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23f8879fcde6014a5291228dc40b0b44f790fad0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976641"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAward personAward = graphClient.me().profile().awards("{id}")
    .buildRequest()
    .get();

```