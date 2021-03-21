---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6517c1083234916b0ccb275dd2f81e8d201030b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976759"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{user-id}")
    .buildRequest()
    .delete();

```