---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbb63c668bf9a15c5c4169ede8be69974b0def59
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations')
    .get();

```