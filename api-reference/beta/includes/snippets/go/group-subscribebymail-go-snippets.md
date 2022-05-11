---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6fbfc3e3a73e1e77b8686132dbdf66b863b619af
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322298"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
graphClient.GroupsById(&groupId).SubscribeByMail(group-id).Post()


```