---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39435801dfbcaa01d20ddc945c1b0ef3e1b6c669
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953416"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintJobCollectionPage jobs = graphClient.print().shares("{printerShareId}").jobs()
    .buildRequest()
    .get();

```