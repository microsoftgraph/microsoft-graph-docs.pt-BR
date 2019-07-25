---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f326ca7ff961de9878836c57211a9dd20fe779d9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877594"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolder outlookTaskFolder = graphClient.me().outlook().taskFolders("AAMkADIyAAAAABrJAAA=")
    .buildRequest()
    .get();

```