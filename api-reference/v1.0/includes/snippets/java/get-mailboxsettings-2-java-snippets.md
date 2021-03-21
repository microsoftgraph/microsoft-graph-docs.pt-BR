---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a26490d650ff0eafe029e2aef7f12202c0a7c9ea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975893"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AutomaticRepliesSetting automaticRepliesSetting = graphClient.customRequest("/me/mailboxSettings/automaticRepliesSetting", AutomaticRepliesSetting.class)
    .buildRequest()
    .get();

```