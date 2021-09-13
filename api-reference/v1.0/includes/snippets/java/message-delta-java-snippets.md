---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba27a30e811cb2555775241e2f052d29edd9adea6c1d0e12784d69cc16c3c909
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158953"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "odata.maxpagesize=2"));

MessageDeltaCollectionPage delta = graphClient.me().mailFolders("{id}").messages()
    .delta()
    .buildRequest( requestOptions )
    .get();

```