---
title: tipo de recurso credentialUserRegistrationDetails
description: Representa os detalhes do uso da redefinição de senha de autoatendados e da autenticação multifatória (MFA) para todos os usuários registrados.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ac5712bf3c0d396f7ddc84c4812b4e1ed7090355
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941810"
---
# <a name="credentialuserregistrationdetails-resource-type"></a>tipo de recurso credentialUserRegistrationDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes do uso da redefinição de senha de autoatendados e da autenticação multifatória (MFA) para todos os usuários registrados. Os detalhes incluem informações do usuário, status do registro e o método de autenticação usado.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md) | coleção credentialUserRegistrationDetails | Obter uma lista de [objetos credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) para um determinado locatário.
 |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| authMethods | coleção registrationAuthMethod | Representa o método de autenticação que o usuário registrou. Os valores possíveis são: , , (usado apenas para redefinição de senha de `email` `mobilePhone` `officePhone`  `securityQuestion` autoatendido), , , (suportado somente `appNotification` no  `appCode` `alternateMobilePhone` registro), , ,  `fido`  `appPassword`  `unknownFutureValue` . |
| id | Cadeia de caracteres | O identificador exclusivo da atividade. Somente leitura.|
| isCapable | Booliano | Indica se o usuário está pronto para executar a redefinição de senha de autoatendados ou MFA. |
| isEnabled | Booliano | Indica se o usuário habilitado para executar a redefinição de senha de autoatendados. |
| isMfaRegistered | Booliano | Indica se o usuário está registrado para MFA. |
| isRegistered | Booliano | Indica se o usuário registrou quaisquer métodos de autenticação para redefinição de senha de autoatendados. |
| userDisplayName | Cadeia de caracteres | Fornece o nome de usuário do usuário correspondente. |
| userPrincipalName | Cadeia de caracteres | Fornece o nome principal do usuário do usuário correspondente. |

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


