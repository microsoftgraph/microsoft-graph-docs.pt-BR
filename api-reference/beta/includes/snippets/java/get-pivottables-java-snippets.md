---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54b1e50dc42397bd0c590731e86fb9e4b4d5a2bac401268e5ad892f1c4e99490
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215134"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookPivotTableCollectionPage pivotTables = graphClient.drive().root().workbook().worksheets("{id}").pivotTables()
    .buildRequest()
    .get();

```