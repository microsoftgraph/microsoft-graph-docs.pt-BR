---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5af907d1df924f7b3409f0d3e2cbb1e0227954fd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113571"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration()
    .buildRequest()
    .delete();

```