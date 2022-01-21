---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb72ed6baee3bcb17fd56952c458571a1ffb0ed6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116617"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BaseTaskList baseTaskList = graphClient.me().tasks().lists("AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAADG6BbDxY")
    .buildRequest()
    .get();

```