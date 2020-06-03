---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8683360bd5b5e7a75e59e09669c26d66326fede1
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/callRecords/{id}/sessions')
    .version('beta')
    .get();

```