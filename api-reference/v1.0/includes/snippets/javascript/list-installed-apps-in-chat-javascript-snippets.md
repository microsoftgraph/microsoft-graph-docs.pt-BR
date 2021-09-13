---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07816670126ab5ce87e8b3a31aed1ab67ff093d961f6fd1ac83c78857c2931f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps')
    .get();

```