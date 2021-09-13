---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41cbb96cec59aca889575bbd37c6140ec8221358765bdcfa91aed5ad28ce7d4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214354"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShift = await client.api('/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8')
    .get();

```