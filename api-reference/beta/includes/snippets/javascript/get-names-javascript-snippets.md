---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb98eb094a81e3db2d59b887155c08ee44e0ac3c
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50178990"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/names')
    .version('beta')
    .get();

```