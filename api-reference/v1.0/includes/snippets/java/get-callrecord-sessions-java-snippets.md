---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d58d02bbdebaa9bd99bfc9d398cec0e8b0c6f0f3
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524559"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISessionCollectionPage sessions = graphClient.communications().callRecords("{id}").sessions()
    .buildRequest()
    .get();

```