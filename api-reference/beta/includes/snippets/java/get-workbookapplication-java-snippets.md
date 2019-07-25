---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf9d21794a826b5f0a4afa64a51131f5be466af2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866456"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookApplication workbookApplication = graphClient.me().drive().items("{id}").workbook().application()
    .buildRequest()
    .get();

```