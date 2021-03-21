---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a833a3ffb336ef4b2494b2c25e6dd4636bb7a7b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971311"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}")
    .buildRequest()
    .delete();

```