---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf55648617be9f9c966b127bea4ab373527c42d7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972950"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().positions("{id}")
    .buildRequest()
    .delete();

```