---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6a6dca53160b22f8f83d368d86a2637fbef1bb52a64ebf5fc4d8dd029efea58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271802"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemEmailCollectionPage emails = graphClient.me().profile().emails()
    .buildRequest()
    .get();

```