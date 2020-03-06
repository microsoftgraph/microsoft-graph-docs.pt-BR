---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f80ab2fe4e2f151757279a4eb78492b18357dd79
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997145"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications')
    .get();

```