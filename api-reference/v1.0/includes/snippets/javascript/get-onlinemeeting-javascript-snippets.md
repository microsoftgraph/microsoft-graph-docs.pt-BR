---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef53edb698ceaf38b1a19896b3ca9717677b375c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465400"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/onlineMeetings/')
    .filter('VideoTeleconferenceId eq \'123456789\'')
    .get();

```