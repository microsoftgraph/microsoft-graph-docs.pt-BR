---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00f7a180280ce575566af360459bb00e4a883cd2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804506"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryObject = await client.api('/directoryObjects/{id}')
    .version('beta')
    .get();

```