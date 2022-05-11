---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9119664ab8ea160744afe8197f53668d2ee68a7e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323422"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().FindRooms()().Get()


```