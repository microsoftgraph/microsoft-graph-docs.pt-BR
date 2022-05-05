---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95bd4e947a85df74451dd3d659e9eccdae560326
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211772"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Remove-MgDomainFederationConfiguration -DomainId $domainId -InternalDomainFederationId $internalDomainFederationId

```