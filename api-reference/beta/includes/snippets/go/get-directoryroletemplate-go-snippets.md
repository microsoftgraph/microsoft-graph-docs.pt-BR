---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35476237113dbdcf0fe87f516660f386453d9910
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286074"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directoryRoleTemplateId := "directoryRoleTemplate-id"
result, err := graphClient.DirectoryRoleTemplatesById(&directoryRoleTemplateId).Get(nil)


```