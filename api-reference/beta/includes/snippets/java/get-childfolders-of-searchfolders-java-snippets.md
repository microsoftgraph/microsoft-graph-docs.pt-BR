---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: daba38f45260b401e2d8eba3da39ca532b34d1b6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979345"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailFolderCollectionPage childFolders = graphClient.me().mailFolders("searchfolders").childFolders()
    .buildRequest()
    .get();

```