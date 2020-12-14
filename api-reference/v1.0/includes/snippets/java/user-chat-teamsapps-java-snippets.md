---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4edb53353751fb73c8334ea6fc0e4da03cf655d2
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49656992"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.users("{id}").teamwork().installedApps("{id}").chat()
    .buildRequest()
    .get();

```