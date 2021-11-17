---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4210facc182e53f3276c45c9b9887c569f8b8c0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "61020368"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SoftwareOathAuthenticationMethod softwareOathAuthenticationMethod = graphClient.me().authentication().softwareOathMethods("b172893e-893e-b172-3e89-72b13e8972b1")
    .buildRequest()
    .get();

```