---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 913a7f648ab7dcb1d5cd376493dd421f783da703
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980310"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "displayName-value";

graphClient.me().mailFolders()
    .buildRequest()
    .post(mailFolder);

```