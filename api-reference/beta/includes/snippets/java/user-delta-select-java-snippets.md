---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50588df1d56aa925de2c0a4b3f3d1d9559ff292d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979087"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserDeltaCollectionPage delta = graphClient.users()
    .delta()
    .buildRequest()
    .select("displayName,jobTitle,mobilePhone")
    .get();

```