---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9837f3f644031111acdbd735dfc4ad9111f0584
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740323"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels')
    .get();

```