---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57c61828ea52cb1c218d1ca6f3ccd1bef90fe86e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968161"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().taskDefinitions("4c6a0f26-8e5d-4bf6-91e6-4a5731adec19")
    .buildRequest()
    .delete();

```