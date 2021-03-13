---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f50cfd7725e4549881826dce826a10788fcd967f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771999"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintConnectorCollectionPage connectors = graphClient.print().connectors()
    .buildRequest()
    .get();

```