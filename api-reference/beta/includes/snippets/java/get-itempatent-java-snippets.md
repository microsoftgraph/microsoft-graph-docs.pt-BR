---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9766cfd363d92dcab0a0a52b8b0150f8513d1a92
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984076"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPatent itemPatent = graphClient.me().profile().patents("{id}")
    .buildRequest()
    .get();

```