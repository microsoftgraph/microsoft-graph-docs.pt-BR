---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 041ca750c2b578950d56d12f7ada0143c35330046eb0caea35c838944ec71713
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159157"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels("19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2").messages("1612509044972").replies("1613671348387")
    .buildRequest()
    .get();

```