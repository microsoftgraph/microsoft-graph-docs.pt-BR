---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b40e4faf4e25fe28aaa64995c4650a553cd42733fc274f2f41948131917bf1cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275138"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBrandingLocalization organizationalBrandingLocalization = new OrganizationalBrandingLocalization();
organizationalBrandingLocalization.backgroundColor = "#00000F";
organizationalBrandingLocalization.signInPageText = "fr";

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding().localizations("fr")
    .buildRequest()
    .put(organizationalBrandingLocalization);

```