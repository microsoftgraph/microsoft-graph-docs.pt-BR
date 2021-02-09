---
title: Tipo de recurso credentialUserRegistrationDetails
description: Representa os detalhes do uso da redefinição de senha de autoatendado e da autenticação multifatória (MFA) para todos os usuários registrados.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c7e45b186e1ef7a3a96115f408cb5a0992e538fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159903"
---
# <a name="credentialuserregistrationdetails-resource-type"></a>Tipo de recurso credentialUserRegistrationDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes do uso da redefinição de senha de autoatendado e da autenticação multifatória (MFA) para todos os usuários registrados. Os detalhes incluem informações do usuário, status do registro e o método de autenticação usado.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md) | Coleção credentialUserRegistrationDetails | Obter uma lista de [objetos credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.
 |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| authMethods | Coleção registrationAuthMethod | Representa o método de autenticação que o usuário registrou. Os valores possíveis são: , , (usado somente para redefinição de senha de `email` `mobilePhone` `officePhone` `securityQuestion` autoatendido) e (com suporte `appNotification` apenas no `appCode` `alternateMobilePhone` registro). |
| id | String | O identificador exclusivo da atividade. Somente leitura.|
| isCapable | Boolean | Indica se o usuário está pronto para executar a redefinição de senha de autoatendado ou a MFA. |
| isEnabled | Booliano | Indicia se o usuário está habilitado para executar a redefinição de senha de autoatendência. |
| isMfaRegistered | Boolean | Indicia se o usuário está registrado para MFA. |
| isRegistered | Boolean | Indica se o usuário registrou quaisquer métodos de autenticação para redefinição de senha de autoatendado. |
| userDisplayName | Cadeia de caracteres | Fornece o nome de usuário do usuário correspondente. |
| userPrincipalName | String | Fornece o nome principal do usuário do usuário correspondente. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "authMethods": ["string"],
  "isRegistered" : false,
  "isEnabled" : true,
  "isCapable" : false,
  "isMfaRegistered" : true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


