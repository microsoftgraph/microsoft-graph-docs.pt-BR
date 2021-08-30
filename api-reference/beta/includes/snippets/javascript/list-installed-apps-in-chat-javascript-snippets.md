---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7fb8449148079fb0705243b44bada845e0a6b349885cf195d3ad5648cb301256
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps')
    .version('beta')
    .get();

```