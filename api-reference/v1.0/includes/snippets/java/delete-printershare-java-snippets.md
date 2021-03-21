---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2df48dc39538d226601d90576eec34ba456b257b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970209"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{printerShareId}")
    .buildRequest()
    .delete();

```