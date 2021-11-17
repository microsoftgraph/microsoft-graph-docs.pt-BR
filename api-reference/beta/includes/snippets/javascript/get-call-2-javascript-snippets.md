---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a83102866f7adce7599fd0a6762d339eab369ad6c4b1240cca4f5b331eac127c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156273"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let call = await client.api('/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92')
    .version('beta')
    .get();

```