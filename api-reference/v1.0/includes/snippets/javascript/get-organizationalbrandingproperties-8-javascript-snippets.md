---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe4e3d608bc8a45df2a1fa0e9e559d0b1e6986c6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBrandingLocalization = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr')
    .get();

```