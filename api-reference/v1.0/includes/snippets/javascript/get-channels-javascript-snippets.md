---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9837f3f644031111acdbd735dfc4ad9111f0584
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35491960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels')
    .get();

```