---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dba6252a13079c34d99d13090049e5642f41a1ea
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904460"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.teams("303d2c1c-f1c5-40ce-b68e-544343d7f42b").channels("19:fec4b0f2825d4c8c82abc09027a64184@thread.skype").messages("1555375673184").replies("1555377090002")
    .buildRequest()
    .get();

```