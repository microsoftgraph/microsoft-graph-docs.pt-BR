---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 094e2b4550c559a8e701498be82d532ca7edb0640e6b4628a861a34049da9a40
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899699"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh')
    .post();

```