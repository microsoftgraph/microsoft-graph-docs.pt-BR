---
title: claimsMapping tipo de recurso
description: Mapeie as declarações de um token para as declarações que o Azure Active Directory B2C reconhece e usa.
author: namkedia
ms.localizationpriority: high
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3862cf564ce5df1924972e75dfb22a3ba0756429
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696208"
---
# <a name="claimsmapping-resource-type"></a>claimsMapping tipo de recurso

Namespace: Microsoft Graph

Depois que o provedor de identidade personalizado envia um token de ID de volta ao Azure AD B2C, o Azure AD B2C mapeia as declarações de um token para as declarações que o Azure AD B2C reconhece e usa.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:-------|:---|:----------|
|userId|Cadeia de caracteres|A declaração que fornece o identificador exclusivo para o usuário conectado. É uma propriedade necessária.|
|displayName|Cadeia de caracteres|A declaração que fornece o nome de exibição ou o nome completo do usuário. É uma propriedade necessária.|
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


