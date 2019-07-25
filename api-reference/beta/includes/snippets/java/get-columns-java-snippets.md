---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b44186ce42eb60f2af471943842aea13ed1076bc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868920"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$skip", "5"));

IWorkbookTableColumnCollectionPage columns = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .buildRequest( requestOptions )
    .top(5)
    .get();

```