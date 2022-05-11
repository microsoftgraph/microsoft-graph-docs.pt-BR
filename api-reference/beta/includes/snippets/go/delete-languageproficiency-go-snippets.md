---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7269653cf6544a6ab757fbd56f2fd3411c454518
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324934"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

languageProficiencyId := "languageProficiency-id"
graphClient.Me().Profile().LanguagesById(&languageProficiencyId).Delete()


```