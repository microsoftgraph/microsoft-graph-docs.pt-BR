---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60dbe13f62d05924684a7e687a40ee1f50d73c0c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397292"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSettingCollectionPage settings = graphClient.groups("05aa6a98-956a-45c0-b13b-88076a23f2cd").settings()
    .buildRequest()
    .get();

```