---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a9080995c4b4c278e88e9291e27f944aa33ce7b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996407"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schema = await graphClient.External.Connections["contosohr"].Schema
    .Request()
    .GetAsync();

```