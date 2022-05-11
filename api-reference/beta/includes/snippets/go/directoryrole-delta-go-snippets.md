---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61e65e0cd777a9f8726a52d73db7f850e08b506f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324347"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.DirectoryRoles().Delta()().Get()


```