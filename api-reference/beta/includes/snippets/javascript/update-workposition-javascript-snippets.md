---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5bcfbf72b0074ab9d4ba5ca3a901dec3986fe0e0
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821302"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workPosition = {
  isCurrent: true
};

let res = await client.api('/me/profile/positions/{id}')
    .version('beta')
    .update(workPosition);

```