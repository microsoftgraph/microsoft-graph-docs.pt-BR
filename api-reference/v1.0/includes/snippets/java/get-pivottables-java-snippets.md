---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b89e694b1302f7ff6894ee923d914b872af55ca5e8f2a6aefe630960b59eb6a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099922"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookPivotTableCollectionPage pivotTables = graphClient.me().drive().root().workbook().worksheets("{id}").pivotTables()
    .buildRequest()
    .get();

```