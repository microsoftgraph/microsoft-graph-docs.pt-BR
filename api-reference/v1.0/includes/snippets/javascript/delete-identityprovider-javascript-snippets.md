---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 396fee202c9d61260f8c73a0cd833b9856fed7da
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders/Amazon-OAuth')
    .delete();

```