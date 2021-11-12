---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ef25cf77ecc867af1453508562cb2c7ddcc95a6fe37a08abffb9d83ab9510ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217573"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LicenseDetailsCollectionPage licenseDetails = graphClient.me().licenseDetails()
    .buildRequest()
    .get();

```