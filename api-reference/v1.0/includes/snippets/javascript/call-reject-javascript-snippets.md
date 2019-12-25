---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f161233a3b14beb660b24bcb2635897b8c4ff3bd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865716"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reject = {
  reason: "busy"
};

let res = await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject')
    .post(reject);

```