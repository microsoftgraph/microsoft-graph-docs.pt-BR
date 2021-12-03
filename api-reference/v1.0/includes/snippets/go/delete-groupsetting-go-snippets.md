---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d726cca8677556a1c8da84b484c95d197c51cdf9
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287142"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupSettingId := "groupSetting-id"
graphClient.GroupSettingsById(&groupSettingId).Delete(nil)


```