---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b9924e2937e887f9ff80478e60441ba601e129f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436225"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    BaseType = "microsoft.graph.externalItem"
    Properties = @(
        @{
            Name = "ticketTitle"
            Type = "string"
            IsSearchable = "true"
            IsRetrievable = "true"
            Labels = @(
                "title"
            )
        }
        @{
            Name = "priority"
            Type = "string"
            IsQueryable = "true"
            IsRetrievable = "true"
            IsSearchable = "false"
        }
        @{
            Name = "assignee"
            Type = "string"
            IsRetrievable = "true"
        }
    )
}

Update-MgExternalConnectionSchema -ExternalConnectionId $externalConnectionId -BodyParameter $params

```