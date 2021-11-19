---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df3f24cfc0e7659c397839390e72f8499be204ec
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103072"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

subscriptionId := "subscription-id"
graphClient.SubscriptionsById(&subscriptionId).Delete(options)


```