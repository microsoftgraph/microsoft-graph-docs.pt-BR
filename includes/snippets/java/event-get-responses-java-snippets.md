---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 378ac26d1431c8b6b2156cb9077ce157ed596191e9c447144d26c7ad56d77d06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129722"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = graphClient.me().calendar().events("AAMkADJXJGu0AABf02qwAAA=")
    .buildRequest()
    .get();

```