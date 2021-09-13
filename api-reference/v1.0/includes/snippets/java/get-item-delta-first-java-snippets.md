---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 894ac3a4e715e1971e61cd184991b66f259ba02350f6ead09723fb8fad22d482
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898970"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
    .delta()
    .buildRequest()
    .get();

```