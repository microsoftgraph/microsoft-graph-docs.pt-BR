---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5af19e35ccef610d478712514d82fead54a5165
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867813"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

IUserDeltaCollectionPage delta = graphClient.users()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName,jobTitle,mobilePhone")
    .get();

```