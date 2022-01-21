---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78bec3f503e41322323cc04b7deee8b40b0a349b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106134"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgApplicationFederatedIdentityCredential -ApplicationId $applicationId -FederatedIdentityCredentialId $federatedIdentityCredentialId

```