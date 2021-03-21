---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15ddb78e02adb5d8272835a54c27fb1c4d558541
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981478"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().calendarGroups("{id}")
    .buildRequest()
    .delete();

```