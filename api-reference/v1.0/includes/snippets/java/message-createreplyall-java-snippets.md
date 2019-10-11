---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fee1934a19a947e1ada7d2b936fd8fa47a93465c
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428761"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createReplyAll(null,null)
    .buildRequest()
    .post();

```