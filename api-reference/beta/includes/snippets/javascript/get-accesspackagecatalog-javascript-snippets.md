---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 181e87a7b4177c1e4b2ff583d10bd68fa7c3dd52
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994350"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}')
    .version('beta')
    .get();

```