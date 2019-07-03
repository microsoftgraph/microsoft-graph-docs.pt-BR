---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3183b33260b7ed6f53db72e07dd4f8f37c6816fd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timesOff/{timeOffId}')
    .version('beta')
    .get();

```