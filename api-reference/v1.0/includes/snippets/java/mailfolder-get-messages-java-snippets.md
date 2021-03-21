---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81f098889f7c512130bde74a5482d02c4fdaf769
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967136"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageCollectionPage messages = graphClient.me().mailFolders("{id}").messages()
    .buildRequest()
    .get();

```