---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbe1d9b6a1985acf2b240351e172981d64c1dd65
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62530496"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Admin().Windows().Updates().UpdatableAssets().Get(nil)


```