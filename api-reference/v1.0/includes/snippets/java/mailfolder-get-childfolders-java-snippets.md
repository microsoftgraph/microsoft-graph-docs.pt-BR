---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8e0f07b739dbe5aad785583c03a8c3fa0fb7990
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976119"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolderCollectionPage childFolders = graphClient.me().mailFolders("{id}").childFolders()
    .buildRequest()
    .get();

```