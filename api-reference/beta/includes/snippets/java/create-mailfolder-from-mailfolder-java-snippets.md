---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0cfe1b5b504f0385a00825bb5b786f732487dfe3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879954"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "displayName-value";

graphClient.me().mailFolders("{id}").childFolders()
    .buildRequest()
    .post(mailFolder);

```