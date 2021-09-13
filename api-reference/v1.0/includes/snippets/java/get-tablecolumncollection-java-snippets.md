---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ba637d2da56c495f20fbba778156d9c18aa6d5304f4eaa241946c834eda5768
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271786"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableColumnCollectionPage columns = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .buildRequest()
    .get();

```