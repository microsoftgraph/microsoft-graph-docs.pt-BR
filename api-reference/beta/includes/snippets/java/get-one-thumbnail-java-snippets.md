---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78c25d850b053f375e95a0a3825c759bfe358633149b2366127f2d7265297427
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274961"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content response = graphClient.me().drive().items("{item-id}").thumbnails("{thumb-id}").{size}()
    .buildRequest()
    .get();

```