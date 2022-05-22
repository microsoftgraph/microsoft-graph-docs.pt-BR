---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aecd41c2d0eb95e9fae381e580c590e060fcde7d
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629791"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
groupSettingId := "groupSetting-id"
result, err := graphClient.GroupsById(&groupId).SettingsById(&groupSettingId).Get()


```