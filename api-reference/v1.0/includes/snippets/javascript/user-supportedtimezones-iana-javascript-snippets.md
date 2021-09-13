---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eeff646d7546f9957b6924290dfb54e9d9761d8967cc8560fd55757d91e9646b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327473"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let supportedTimeZones = await client.api('/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')')
    .get();

```