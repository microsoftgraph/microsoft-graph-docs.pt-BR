---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 405d3bf0a42253a9b43dadc247ff2ead13e66954e4673623d4cdccb36a7ec0eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273527"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .usedRange()
    .buildRequest()
    .get();

```