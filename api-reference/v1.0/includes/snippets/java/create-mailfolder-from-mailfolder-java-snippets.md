---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67867bdc1ea2c33fd88ee24d529b408d9a60f6a790244695411d4d0773d32f84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275307"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "displayName-value";
mailFolder.isHidden = true;

graphClient.me().mailFolders("{id}").childFolders()
    .buildRequest()
    .post(mailFolder);

```