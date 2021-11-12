---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87db8eff0738a812012d7cf784ce4913fe42363b46a3810425493c45914b8c74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214786"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .buildRequest()
    .get();

```