---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e84d719a75d22bf6754cafbc8d1fa66534b01669
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/callRecords/{id}/sessions')
    .version('beta')
    .expand('segments')
    .get();

```