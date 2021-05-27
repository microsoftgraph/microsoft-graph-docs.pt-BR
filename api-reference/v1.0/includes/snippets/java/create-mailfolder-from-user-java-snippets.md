---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7ad4cbcd53345db1d1060f89b6f2315eafd3cd7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668645"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "Clutter";
mailFolder.isHidden = true;

graphClient.me().mailFolders()
    .buildRequest()
    .post(mailFolder);

```