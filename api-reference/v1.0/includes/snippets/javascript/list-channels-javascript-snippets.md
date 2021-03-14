---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1d578c3b3c9a78b70738732c300aaf6912138b6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799740"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channels = await client.api('/teams/{id}/channels')
    .get();

```