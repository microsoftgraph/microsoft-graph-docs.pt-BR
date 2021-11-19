---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b15c4a3d105dd5473a3aef084d1cc6a3377f5d44
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091979"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

windowsProtectionStateId := "windowsProtectionState-id"
result, err := graphClient.TenantRelationships().ManagedTenants().WindowsProtectionStatesById(&windowsProtectionStateId).Get(options)


```