---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 902ff43fe09b9361cc1c75623f84570ab1729b02
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087656"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
sitePageId := "sitePage-id"
result, err := graphClient.SitesById(&siteId).PagesById(&sitePageId).Get(options)


```