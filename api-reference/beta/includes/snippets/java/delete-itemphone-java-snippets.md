---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 683d86ebba25511cf6cf01a35bd19193bb0cc3d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981550"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().phones("{itemPhoneId}")
    .buildRequest()
    .delete();

```