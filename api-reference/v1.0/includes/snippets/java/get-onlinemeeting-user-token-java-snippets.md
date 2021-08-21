---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23deaece6323f791953badd534e6d4c3b0fdf7c058a40b9aebba6a1039565912
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159247"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy")
    .buildRequest()
    .get();

```