---
title: claimsMapping tipo de recurso
description: Mapeie as declarações de um token para as declarações que o Azure Active Directory B2C reconhece e usa.
author: namkedia
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 07e2d7a008db5377869d12d426d8d3d1e440a40c
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534092"
---
# <a name="claimsmapping-resource-type"></a>claimsMapping tipo de recurso
Namespace: Microsoft Graph

Depois que o provedor de identidade personalizado envia um token de ID de volta ao Azure AD B2C, o Azure AD B2C mapeia as declarações de um token para as declarações que o Azure AD B2C reconhece e usa.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:-------|:---|:----------|
|userId|Cadeia de caracteres|A declaração que fornece o identificador exclusivo para o usuário conectado. Necessário.|
|displayName|Cadeia de caracteres|A declaração que fornece o nome de exibição ou o nome completo do usuário. Necessário.|
|givenName|Cadeia de caracteres|A declaração que fornece o primeiro nome do usuário.|
|surname|Cadeia de caracteres|A declaração que fornece o sobrenome do usuário.|
|email|Cadeia de caracteres|A declaração que fornece o endereço de email do usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.claimsMapping"
}
-->

``` json
{
  "userId": "String",
  "givenName": "String",
  "surname": "String",
  "email": "String",
  "displayName": "String"
  }
```

