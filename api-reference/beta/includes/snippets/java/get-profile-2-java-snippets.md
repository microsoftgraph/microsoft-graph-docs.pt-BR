---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3729ccaf3f9ce2ef46d0c3546e1e8c19fdd4ffd
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210477"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Profile profile = graphClient.me().profile()
    .buildRequest()
    .expand("skills($select=displayName)")
    .get();

```