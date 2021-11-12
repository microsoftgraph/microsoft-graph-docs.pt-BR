---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3871814dce51b581fc2c19eea5847bb84d7c5823643441243b5c5b205048b326
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273532"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.contacts("{id}").manager()
    .buildRequest()
    .get();

```