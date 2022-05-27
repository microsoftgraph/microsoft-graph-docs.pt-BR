---
title: Tipo de recurso userRegistrationDetails
description: Representa o estado dos métodos de autenticação de um usuário, incluindo quais métodos são registrados e quais recursos o usuário é registrado e capaz (como autenticação multifator, redefinição de senha de autoatendimento e autenticação sem senha).
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8c2df96cd680896854866618c10a70aae3e65a37
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694725"
---
# <a name="userregistrationdetails-resource-type"></a>Tipo de recurso userRegistrationDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado dos métodos de autenticação de um usuário, incluindo quais métodos são registrados e quais recursos o usuário é registrado e capaz (como autenticação multifator, redefinição de senha de autoatendimento e autenticação sem senha).

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userRegistrationDetails](../api/authenticationmethodsroot-list-userregistrationdetails.md)|[coleção userRegistrationDetails](../resources/userregistrationdetails.md)|Obtenha uma lista dos [objetos userRegistrationDetails](../resources/userregistrationdetails.md) e suas propriedades.|
|[Obter userRegistrationDetails](../api/userregistrationdetails-get.md)|[userRegistrationDetails](../resources/userregistrationdetails.md)|Leia as propriedades e as relações de um [objeto userRegistrationDetails](../resources/userregistrationdetails.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|defaultMfaMethod|defaultMfaMethodType|O método selecionado pelo usuário ou administrador como padrão para executar a autenticação multifator para o usuário. Os valores possíveis são `none`, `mobilePhone`, `alternateMobilePhone`, `officePhone`, `microsoftAuthenticatorPush`, `softwareOneTimePasscode`, `unknownFutureValue`.|
|id|Cadeia de caracteres|Identificador de objeto de usuário Azure AD. Herdado da [entidade](../resources/entity.md).|
|isMfaCapable|Booliano|Se o usuário registrou um método de autenticação forte para autenticação multifator. O método deve ser permitido pela política [de métodos de autenticação](../resources/authenticationmethodspolicy.md). Suporta `$filter` (`eq`).|
|isMfaRegistered|Booliano|Se o usuário registrou um método de autenticação forte para autenticação multifator. O método pode não ser necessariamente permitido pela política [de métodos de autenticação](../resources/authenticationmethodspolicy.md).  Suporta `$filter` (`eq`).|
|isPasswordlessCapable|Booliano|Se o usuário registrou um método de autenticação forte sem senha (incluindo FIDO2, Windows Hello para Empresas e Microsoft Authenticator (sem senha)) permitido pela política de métodos [de autenticação](../resources/authenticationmethodspolicy.md). Suporta `$filter` (`eq`).|
|isSsprCapable|Booliano|Se o usuário registrou o número necessário de métodos de autenticação para redefinição de senha de autoatendimento e se o usuário tem permissão para executar a redefinição de senha de autoatendimento por política. Suporta `$filter` (`eq`).|
|isSsprEnabled|Booliano|Se o usuário tem permissão para executar a redefinição de senha por autoatendimento por política. O usuário pode não ter necessariamente registrado o número necessário de métodos de autenticação para redefinição de senha de autoatendimento. Suporta `$filter` (`eq`).|
|isSsprRegistered|Booliano|Se o usuário registrou o número necessário de métodos de autenticação para redefinição de senha de autoatendimento. O usuário não pode necessariamente ter permissão para executar a redefinição de senha por autoatendimento por política. Suporta `$filter` (`eq`).|
|methodsRegistered|Coleção de cadeias de caracteres|Coleção de métodos de autenticação registrados, como `mobilePhone`, `email`, `fido2`. Dá `$filter` suporte (`any` com `eq`).|
|userDisplayName|Cadeia de caracteres| O nome de exibição do usuário, como `Adele Vance`. Dá `$filter` suporte a (`eq`, `startsWith`) e `$orderBy`.|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário, como `AdeleV@contoso.com`. Dá `$filter` suporte a (`eq`, `startsWith`) e `$orderBy`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userRegistrationDetails",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationDetails",
  "defaultMethod": "String",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "isMfaRegistered": "Boolean",
  "isMfaCapable": "Boolean",
  "isSsprRegistered": "Boolean",
  "isSsprEnabled": "Boolean",
  "isSsprCapable": "Boolean",
  "isPasswordlessCapable": "Boolean",
  "methodsRegistered": [
    "String"
  ]
}
```

