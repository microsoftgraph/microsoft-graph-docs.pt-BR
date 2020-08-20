---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9171146746a2db77930e6cabfc8d13d79bd904ca
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/awards')
    .version('beta')
    .get();

```