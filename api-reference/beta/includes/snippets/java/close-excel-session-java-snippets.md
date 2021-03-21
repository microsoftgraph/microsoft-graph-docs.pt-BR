---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6df1b70581bd6081f11f55df4088a3b24345fdf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983520"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("workbook-session-id", "{session-id}"));

graphClient.me().drive().items("{id}").workbook()
    .closeSession()
    .buildRequest( requestOptions )
    .post();

```