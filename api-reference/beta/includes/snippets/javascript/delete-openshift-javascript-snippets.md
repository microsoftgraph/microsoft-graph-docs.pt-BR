---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 638b0a0df2ee4ebd65b1c4d7ff983f02b1e4e32c937dbb791e6e068c20b877a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8')
    .version('beta')
    .delete();

```