---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96949a0701041973cc96a4c0ba50b8095cefbfc9
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944769"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content shiftPreferences = graphClient.users("871dbd5c-3a6a-4392-bfe1-042452793a50").shiftPreferences()
    .buildRequest()
    .get();

```