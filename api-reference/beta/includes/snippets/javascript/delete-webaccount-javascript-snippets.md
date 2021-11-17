---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72bfc2445edf2685fce13f142d2e4de27806e8d3402680ff82c6a587d9d31be9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215140"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/webAccounts/{id}')
    .version('beta')
    .delete();

```