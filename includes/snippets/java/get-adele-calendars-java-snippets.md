---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfa3019e92fb73219fa492397d9ab1ce35e467bf7ef2bb0ac19470e543a6f3c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129719"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICalendarCollectionPage calendars = graphClient.me().calendars()
    .buildRequest()
    .get();

```