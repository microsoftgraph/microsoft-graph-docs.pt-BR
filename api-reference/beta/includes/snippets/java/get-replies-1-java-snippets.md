---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 027843cd219f103e3f6927af8cd3ce53e5aa480d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208555"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageCollectionPage replies = graphClient.chats("{id}").messages("{id}").replies()
    .buildRequest()
    .get();

```