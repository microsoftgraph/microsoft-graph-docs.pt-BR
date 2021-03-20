---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10c3967d5d3dab0c42fde9ffdbcf24bd79a8b3a3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976946"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethod authenticationMethod = graphClient.me().authentication().methods("{id}")
    .buildRequest()
    .get();

```