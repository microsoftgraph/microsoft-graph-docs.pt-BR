---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39cacedebf64e2feb6b9f55675656b974c448d39
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089970"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupSettingId := "groupSetting-id"
graphClient.GroupSettingsById(&groupSettingId).Delete(options)


```