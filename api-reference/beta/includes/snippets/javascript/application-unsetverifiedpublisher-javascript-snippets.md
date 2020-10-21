---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc8069bd459db8602d730fa2438604148745d488
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634675"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/unsetVerifiedPublisher')
    .version('beta')
    .post();

```