---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af604452bd1d884fb441dcebd11eaa53addad02c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779252"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let team = await client.api('/teams/{id}')
    .get();

```