---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1fb8a5af69782a9d44c6b2d1b7a2d348b0846a80
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974097"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailSearchFolder mailFolder = new MailSearchFolder();
mailFolder.filterQuery = "contains(subject, 'Analytics')";

graphClient.me().mailFolders("AAMkAGVmMDEzM")
    .buildRequest()
    .patch(mailFolder);

```