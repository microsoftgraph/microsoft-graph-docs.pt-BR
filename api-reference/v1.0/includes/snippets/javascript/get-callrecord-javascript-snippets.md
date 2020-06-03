---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8545e348305d6973a20b33b4f1bd668a5c22032d
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524611"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/callRecords/{id}')
    .get();

```