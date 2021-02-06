---
title: Tipo de recurso credentialUserRegistrationCount
description: Representa o estado atual de quantos usuários em sua organização estão registrados para redefinição de senha de autoatendado e recursos de autenticação multifa factor.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: cb83bbfe4c738fd8c5c6460a27aafbbc73cad437
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136273"
---
# <a name="credentialuserregistrationcount-resource-type"></a>Tipo de recurso credentialUserRegistrationCount

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado atual de quantos usuários em sua organização estão registrados para redefinição de senha de autoatendado e recursos de autenticação multifa factor.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [getCredentialUserRegistrationCount](../api/reportroot-getcredentialuserregistrationcount.md) | Coleção credentialUserRegistrationCount | Relatar o estado atual de quantos usuários em sua organização estão registrados para redefinição de senha de autoatendado e recursos de autenticação multifatória (MFA). |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| id | String | O identificador exclusivo da atividade. Somente leitura. |
| totalUserCount | Int64 | Fornece a contagem total de usuários no locatário. |
| userRegistrationCounts | [Coleção userRegistrationCount](userregistrationcount.md) | Uma coleção de informações de status e contagem de registro para usuários em seu locatário. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "totalUserCount" : 23123,
  "userRegistrationCounts" :
  [
    { "registrationStatus":"registered", "registrationCount": 23423 },
    { "registrationStatus":"enabled", "registrationCount": 4234 },
    { "registrationStatus":"capable", "registrationCount": 323 },
    { "registrationStatus":"mfaRegistered", "registrationCount": 33 }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

