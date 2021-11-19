---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f51704b9b7515957804516658b90697ca8995fa3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088032"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directorySettingId := "directorySetting-id"
graphClient.SettingsById(&directorySettingId).Delete(options)


```