---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad5dd15c777e861c1bfff72c6636f85b0feb49c3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771747"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{printerShareId}").allowedUsers("{userId}").reference()
    .buildRequest()
    .delete();

```