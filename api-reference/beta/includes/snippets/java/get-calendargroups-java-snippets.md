---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be196384a3d395aef4b03518bbf7ff93e5fd11b472ddefc3b4ebbb73d0af8138
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329557"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroupCollectionPage calendarGroups = graphClient.me().calendarGroups()
    .buildRequest()
    .get();

```