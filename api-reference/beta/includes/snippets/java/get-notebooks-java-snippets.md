---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98c79df62f52774cccd8e152084a430c2cd311d9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878916"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

INotebookCollectionPage notebooks = graphClient.me().onenote().notebooks()
    .buildRequest()
    .get();

```