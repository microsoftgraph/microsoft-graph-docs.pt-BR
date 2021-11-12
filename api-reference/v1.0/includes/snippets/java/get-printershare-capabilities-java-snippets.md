---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3d01e8880b9727ba30665656c8f55f4caff845f2f68f1dc131f640f2209c542
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375951"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = graphClient.print().shares("{printerShareId}")
    .buildRequest()
    .select("id,displayName,capabilities")
    .get();

```