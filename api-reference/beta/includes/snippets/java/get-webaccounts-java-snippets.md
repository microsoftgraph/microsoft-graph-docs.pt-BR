---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf312e90765cf81a1803fb50077a93cda99eeb4ab0f6843746d50c80d57864d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274727"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WebAccountCollectionPage webAccounts = graphClient.me().profile().webAccounts()
    .buildRequest()
    .get();

```