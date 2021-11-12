---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cede169016d02703775bfa6887cbca6ec3478478b3bd776971fde2e944e96bfb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)')
    .version('beta')
    .get();

```