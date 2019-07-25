---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b08e6b5df90e0afb938a469ab52514291fdb5c99
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868535"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookTableRowCollectionPage rows = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows()
    .buildRequest()
    .get();

```