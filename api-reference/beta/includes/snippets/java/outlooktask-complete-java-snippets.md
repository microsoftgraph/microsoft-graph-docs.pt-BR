---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd7318c7eac95c9c96fda856684b4bfa51a78621
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775539"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

graphClient.me().outlook().tasks("AAMkADA1MT15rfAAA=")
    .complete()
    .buildRequest( requestOptions )
    .post();

```