---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5e950f7d7a322e3b918be4c3cfadcb7573caf8b
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216575"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOpenShiftCollectionPage openShifts = graphClient.teams("{id}").schedule().openShifts()
    .buildRequest()
    .get();

```