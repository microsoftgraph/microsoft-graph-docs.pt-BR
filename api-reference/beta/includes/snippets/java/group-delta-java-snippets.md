---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81d6d09e4dcc63302e7d44a167272ad68a48d685c727b05b526d7ddd68ea2511
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214563"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupDeltaCollectionPage delta = graphClient.groups()
    .delta()
    .buildRequest()
    .get();

```