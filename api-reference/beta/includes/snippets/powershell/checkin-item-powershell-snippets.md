---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fdf5751cb4b1a6e4f0bb0a6c6aa2499ec83ee7ff
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445661"
---
```powershell

Import-Module Microsoft.Graph.Files

$params = @{
    Comment = "Updating the latest guidelines"
}

Invoke-MgCheckinDriveItem -DriveId $driveId -DriveItemId $driveItemId -BodyParameter $params

```