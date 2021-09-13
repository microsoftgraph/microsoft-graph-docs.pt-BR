---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1b7e9e48c7f1ffe0e67a41e3a7c5674cc298a54d8ead9be0d39256ad1069cf7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: 'Volunteer'
};

await client.api('/me/calendars')
    .post(calendar);

```