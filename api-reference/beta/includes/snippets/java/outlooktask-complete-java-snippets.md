---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 425be3c1cee62c97530d4ba0a70b8a773c23da66
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982235"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

graphClient.me().outlook().tasks("AAMkADA1MT15rfAAA=")
    .complete()
    .buildRequest( requestOptions )
    .post();

```