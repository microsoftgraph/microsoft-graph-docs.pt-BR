---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be8af76388e6fea483512ccfc9c0044b1b6a67a5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975778"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolder contactFolder = new ContactFolder();
contactFolder.parentFolderId = "parentFolderId-value";
contactFolder.displayName = "displayName-value";

graphClient.me().contactFolders()
    .buildRequest()
    .post(contactFolder);

```