---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57473cbb142913cac15f7cc69b15304a822415f3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/special/{special-folder-name}/children')
    .get();

```