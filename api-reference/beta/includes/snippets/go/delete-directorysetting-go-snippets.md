---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe8211c16eaa3709efd48e605d6932dbd54d19cc
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286071"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directorySettingId := "directorySetting-id"
graphClient.SettingsById(&directorySettingId).Delete(nil)


```