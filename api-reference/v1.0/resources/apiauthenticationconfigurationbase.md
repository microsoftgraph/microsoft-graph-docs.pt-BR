---
title: Tipo de recurso apiAuthenticationConfigurationBase
description: Representa o tipo base de configuração de autenticação usado para chamar uma API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c897bc970fc4527a03593a72e1ea760ab78fc696a75180e0e718a81ab90455ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54150042"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a>Tipo de recurso apiAuthenticationConfigurationBase

Namespace: microsoft.graph

O tipo base para manter informações de autenticação para chamar uma API.

Os tipos derivados incluem:
- [basicAuthentication para](basicauthentication.md) autenticação básica HTTP
- [pkcs12certificate para autenticação](pkcs12certificate.md) de certificado do cliente (usado para criar ou carregar conectores de API)
- [clientCertificateAuthentication para](pkcs12certificate.md) autenticação de certificado de cliente (usado para buscar os certificados do cliente de um conector de API)

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.apiAuthenticationConfigurationBase"
}
```
