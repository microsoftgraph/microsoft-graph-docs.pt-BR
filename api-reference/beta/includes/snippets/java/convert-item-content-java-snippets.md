---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b98e6b5c4b82d32c971dcf59f2cd0252fed41bae
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971200"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("format", "{format}"));

InputStream stream = graphClient.customRequest("/drive/items/{item-id}/content", InputStream.class)
    .buildRequest( requestOptions )
    .get();

```