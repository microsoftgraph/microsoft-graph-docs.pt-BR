---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82f13a4b1796c4a19fcedcdee098aa8e967fe132
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027730"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupSettingId := "groupSetting-id"
graphClient.GroupSettingsById(&groupSettingId).Delete(options)


```