---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81be720cdbbbd42b304c8776bc1a36ca06da1eb0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979811"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PostCollectionPage posts = graphClient.groups("{id}").threads("{id}").posts()
    .buildRequest()
    .get();

```