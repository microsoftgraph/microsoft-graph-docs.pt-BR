---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abaf4c0614bbbaedb1d6f427390b64facc752eb38bb2795daf20eb9e60f5833e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217273"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let events = await client.api('/me/calendar/events')
    .get();

```