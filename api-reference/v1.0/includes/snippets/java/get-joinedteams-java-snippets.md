---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 773bdcbee41116f346c2f63a096c0c6a51c12df3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982500"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamCollectionPage joinedTeams = graphClient.me().joinedTeams()
    .buildRequest()
    .get();

```