---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20d4bb5cf9a60e7fab4bb37673aba1d91a180a09
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771621"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = graphClient.print().shares("{printerShareId}")
    .buildRequest()
    .select("id,displayName,capabilities")
    .get();

```