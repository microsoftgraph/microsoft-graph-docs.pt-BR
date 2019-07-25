---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c908f4c964ad57875adc91d18cb944798629c34f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872458"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessActivityUserDetailCollectionPage getSkypeForBusinessActivityUserDetail = graphClient.reports()
    .getSkypeForBusinessActivityUserDetail('D7')
    .buildRequest()
    .get();

```