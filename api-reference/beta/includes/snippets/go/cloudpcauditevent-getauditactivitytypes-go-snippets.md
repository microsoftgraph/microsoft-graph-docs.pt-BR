---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd076339dc34e02abbfbcd4395106945c8c66df7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324696"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.DeviceManagement().VirtualEndpoint().AuditEvents().GetAuditActivityTypes()().Get()


```