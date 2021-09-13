---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbda12e487c2047b0def3248c0cb918a0b6b28fa440a87deed289bf9331a1a85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376781"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AutomaticRepliesSetting automaticRepliesSetting = graphClient.customRequest("/me/mailboxSettings/automaticRepliesSetting", AutomaticRepliesSetting.class)
    .buildRequest()
    .get();

```