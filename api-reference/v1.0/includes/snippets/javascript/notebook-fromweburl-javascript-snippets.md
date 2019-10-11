---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6a69097c40d8db23d889beacc31c16dd384257d
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428763"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const copyNotebookModel = {webUrl:"webUrl value"};

let res = await client.api('/me/onenote/notebooks/GetNotebookFromWebUrl')
    .post(copyNotebookModel);

```