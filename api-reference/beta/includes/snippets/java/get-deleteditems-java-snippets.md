---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1014a4856082540abc4ecf08046004c05f817adfc87c545e8faa6ce6d3993ec3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100897"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionPage group = graphClient.directory().deletedItems().microsoft.graph.group()
    .buildRequest()
    .get();

```