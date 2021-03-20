---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99ebf8ea90f08b060659367505eec962b291b15d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978956"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/me/drive/items/{item-id}/content", InputStream.class)
    .buildRequest()
    .get();

```