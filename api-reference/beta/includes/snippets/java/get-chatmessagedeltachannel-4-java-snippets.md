---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c50eb63070ddc34f48b331d4cd113f5e6171f1fc020404e3385d4399a68e6817
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216916"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageDeltaCollectionPage delta = graphClient.teams("fbe2bf47-16c8-47cf-b4a5-4b9b187c508b").channels("19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2").messages()
    .delta()
    .buildRequest()
    .get();

```