---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf83b1e1c2bd0d0610147736c6a32ea9c84946e788c3c03f2c84d027f64550bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275362"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SessionCollectionPage sessions = graphClient.communications().callRecords("{id}").sessions()
    .buildRequest()
    .expand("segments")
    .get();

```