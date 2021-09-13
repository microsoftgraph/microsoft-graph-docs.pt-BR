---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7c4648ff53b16a0ccfbaf046a92188df5aeb27fc5738d75767ae2653ae415d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899566"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachment = await client.api('/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=')
    .get();

```