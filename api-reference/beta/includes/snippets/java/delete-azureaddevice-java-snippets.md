---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 638aa02282eed0490f8bfff2706fc95576faeab2
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241441"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.admin().windows().updates().updatableAssets("{azureADDeviceId}")
    .buildRequest()
    .delete();

```