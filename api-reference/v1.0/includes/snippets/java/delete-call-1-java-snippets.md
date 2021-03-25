---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76b5bfabb9c256bd6044452a60a4db57a106bd53
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209279"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .buildRequest()
    .delete();

```