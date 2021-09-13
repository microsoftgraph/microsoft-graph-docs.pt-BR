---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5d0a71f1bf4df9555efdafab3dfcefc3b4f9f609f020cd5aa46c11bfdaeb844
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive')
    .post();

```