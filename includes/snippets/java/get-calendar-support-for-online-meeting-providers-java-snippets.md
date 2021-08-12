---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36b4c5350b7eec56bb0518e9a1ff4168592eeb4affc50a8495c0baed7716c745
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240496"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar calendar = graphClient.me().calendar()
    .buildRequest()
    .get();

```