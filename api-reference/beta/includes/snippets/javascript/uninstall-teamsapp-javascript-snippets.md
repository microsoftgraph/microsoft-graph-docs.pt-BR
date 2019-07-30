---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed02b2d391a5c98a2231819057626a88bc8aef36
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/installedApps/{id}')
    .version('beta')
    .delete();

```