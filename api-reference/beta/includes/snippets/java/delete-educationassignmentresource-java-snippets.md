---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 233feabf6d66cc6ff93cf46d6b3078c72536f746
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984306"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002").resources("22002")
    .buildRequest()
    .delete();

```