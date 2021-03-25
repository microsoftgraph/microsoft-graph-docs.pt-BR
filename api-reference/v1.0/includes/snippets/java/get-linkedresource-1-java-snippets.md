---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc648d77f348f8a43ae02f1a3ea42df4d545af8f
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208497"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedResource linkedResource = graphClient.me().todo().lists("dfsdc-f9dfdfs-dcsda9").tasks("e2dc-f9cce2-dce29").linkedResources("f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9")
    .buildRequest()
    .get();

```