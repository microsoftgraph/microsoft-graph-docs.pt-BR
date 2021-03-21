---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17773f540b367adcf75486ae64178bfd36a991f8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974159"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolder contactFolder = new ContactFolder();
contactFolder.displayName = "displayName-value";

graphClient.me().contactFolders("{id}").childFolders()
    .buildRequest()
    .post(contactFolder);

```