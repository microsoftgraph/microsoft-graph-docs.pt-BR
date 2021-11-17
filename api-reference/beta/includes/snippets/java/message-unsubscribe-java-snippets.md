---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 404e5fcea764728b37bdf35b32aa044c25a77fa00e1b6177abbe9331b451391a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272845"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .unsubscribe()
    .buildRequest()
    .post();

```