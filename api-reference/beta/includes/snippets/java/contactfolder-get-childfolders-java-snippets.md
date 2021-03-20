---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 205f38920b9ec05e6d60299b76178f0d4c27fcfd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978368"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolderCollectionPage childFolders = graphClient.me().contactFolders("{id}").childFolders()
    .buildRequest()
    .get();

```