---
title: claimsMapping tipo de recurso
description: Mapeie as declarações de um token para as declarações que o Azure Active Directory B2C reconhece e usa.
author: namkedia
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 08fb8b89bd077412275f0a768a8074d669655d179be18ef0910b780a3ab63dfe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189900"
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

