---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50588df1d56aa925de2c0a4b3f3d1d9559ff292d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885753"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserDeltaCollectionPage delta = graphClient.users()
    .delta()
    .buildRequest()
    .select("displayName,jobTitle,mobilePhone")
    .get();

```