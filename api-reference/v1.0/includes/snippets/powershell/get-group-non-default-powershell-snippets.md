---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef26a813bf1a4fa52de0f8d2e96a08a566b5d6ee
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117434"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroup -GroupId $groupId -Property "allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount" 

```