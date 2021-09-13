---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99bcfa9a5e3d160d89449d698a966e35b3333f0f223efa675b868e350c7bbad2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/chats/{id}/members')
    .get();

```