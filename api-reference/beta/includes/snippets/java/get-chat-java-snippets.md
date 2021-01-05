---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70a91b9b875447e390172ea448174a0fc04e2580
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753445"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.users("8b081ef6-4792-4def-b2c9-c363a1bf41d5").chats("19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces")
    .buildRequest()
    .get();

```