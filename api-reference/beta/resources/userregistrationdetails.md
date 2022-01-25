---
title: Tipo de recurso userRegistrationDetails
description: Representa o estado dos métodos de autenticação de um usuário, incluindo quais métodos são registrados e quais recursos o usuário é registrado e capaz (como autenticação multifato, redefinição de senha de autoatendados e autenticação sem senha).
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 11d447b1b4c9069bd4c8d8c29271c4d0b6f51380
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201755"
---
# <a name="userregistrationdetails-resource-type"></a>Tipo de recurso userRegistrationDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado dos métodos de autenticação de um usuário, incluindo quais métodos são registrados e quais recursos o usuário é registrado e capaz (como autenticação multifato, redefinição de senha de autoatendados e autenticação sem senha).

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userRegistrationDetails](../api/authenticationmethodsroot-list-userregistrationdetails.md)|[Coleção userRegistrationDetails](../resources/userregistrationdetails.md)|Obter uma lista dos [objetos userRegistrationDetails](../resources/userregistrationdetails.md) e suas propriedades.|
|[Obter userRegistrationDetails](../api/userregistrationdetails-get.md)|[userRegistrationDetails](../resources/userregistrationdetails.md)|Leia as propriedades e as relações de um [objeto userRegistrationDetails.](../resources/userregistrationdetails.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador de objeto do usuário no Azure AD. Herdado da [entidade](../resources/entity.md).|
|isMfaCapable|Boolean|Se o usuário registrou um método de autenticação forte para autenticação multifato. O método deve ser permitido pela política [de métodos de autenticação](../resources/authenticationmethodspolicy.md). Suporta `$filter` (`eq`).|
|isMfaRegistered|Boolean|Se o usuário registrou um método de autenticação forte para autenticação multifato. O método pode não ser necessariamente permitido pela política de métodos [de autenticação](../resources/authenticationmethodspolicy.md).  Suporta `$filter` (`eq`).|
|isPasswordlessCapable|Boolean|Se o usuário registrou um método de autenticação forte sem senha (incluindo FIDO2, Windows Hello para Empresas e Microsoft Authenticator (Sem Senha)) permitido pela política de métodos de autenticação [.](../resources/authenticationmethodspolicy.md) Suporta `$filter` (`eq`).|
|isSsprCapable|Boolean|Se o usuário registrou o número necessário de métodos de autenticação para redefinição de senha de autoatendados e se o usuário tem permissão para executar a redefinição de senha de autoatendida por política. Suporta `$filter` (`eq`).|
|isSsprEnabled|Boolean|Se o usuário tem permissão para executar a redefinição de senha de autoatendida por política. O usuário pode não ter necessariamente registrado o número necessário de métodos de autenticação para redefinição de senha de autoatendados. Suporta `$filter` (`eq`).|
|isSsprRegistered|Boolean|Se o usuário registrou o número necessário de métodos de autenticação para redefinição de senha de autoatendados. O usuário pode não ter permissão para executar a redefinição de senha de autoatendida por política. Suporta `$filter` (`eq`).|
|methodsRegistered|Coleção de cadeias de caracteres|Coleção de métodos de autenticação registrados, como `mobilePhone` , `email` , `fido2` . Suporta `$filter` ( `any` com `eq` ).|
|userDisplayName|Cadeia de caracteres| O nome de exibição do usuário, como `Adele Vance` . Suporta `$filter` ( , ) e `eq` `startsWith` `$orderBy` .|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário, como `AdeleV@contoso.com` . Suporta `$filter` ( , ) e `eq` `startsWith` `$orderBy` .|

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

