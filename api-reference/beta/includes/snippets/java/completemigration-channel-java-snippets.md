---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4675a08752c0fb0f33ce3ff005f3ffb7b516c57a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974021"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").channels("{channelId}")
    .completeMigration()
    .buildRequest()
    .post();

```