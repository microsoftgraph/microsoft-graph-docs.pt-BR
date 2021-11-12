---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8169802eda0fdb64ba8bba04c3d5a46ad82bb6a781b21054ff53cf24fe49551d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099572"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dailyPrintUsageByPrinter = await client.api('/reports/dailyPrintUsageByPrinter')
    .get();

```