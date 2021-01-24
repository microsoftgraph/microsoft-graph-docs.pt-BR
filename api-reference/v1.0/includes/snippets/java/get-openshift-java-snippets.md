---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cacdc4e62e717f0a84d9d166ba247e7168e3edfa
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946369"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OpenShift openShift = graphClient.teams("{id}").schedule().openShifts("OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8")
    .buildRequest()
    .get();

```