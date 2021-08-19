---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a06f417d6a229a8040bcf616e0fe31c01e65f440284d3967e40ee754f25bbc6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158044"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatCollectionPage chats = graphClient.users("8b081ef6-4792-4def-b2c9-c363a1bf41d5").chats()
    .buildRequest()
    .filter("members/any(o: o/displayname eq 'Peter Parker')")
    .expand("members")
    .get();

```