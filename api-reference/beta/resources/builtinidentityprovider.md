---
title: Tipo de recurso builtInIdentityProvider
description: Representa provedores de identidade internos em um locatário do Azure Active Directory.
ms.localizationpriority: high
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 9905e8974644e55306108cba275a025bac27c7c1
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696229"
---
# <a name="builtinidentityprovider-resource-type"></a>Tipo de recurso builtInIdentityProvider
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa provedores de identidade integrados com [Identidades externas](/azure/active-directory/external-identities/)para um locatário do Azure Active Directory.

Para cenários do Azure AD B2B em um locatário do Azure AD, o tipo de provedor de identidade integrado pode ser um Azure Active Directory (AAD), conta Microsoft (MSA) ou senha única de email (EmailOTP).

Este tipo herdará de [IdentityProviderBase](../resources/identityproviderbase.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/identitycontainer-list-identityproviders.md)|Coleção [identityProviderBase](../resources/identityproviderbase.md) |Recuperar todos os provedores de identidade configurados em um locatário, incluindo os provedores de identidade integrados. Não há como recuperar apenas os provedores de identidade integrados em um locatário.|
|[Get](../api/identityproviderbase-get.md) |builtInIdentityProvider|Recuperar propriedades de um provedor de identidade integrado.|
|[Listar os tipos de provedor disponíveis](../api/identityproviderbase-availableprovidertypes.md)|Coleção de cadeias de caracteres|Recuperar todos os tipos de provedores de identidade disponíveis no locatário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|O identificador do provedor de identidade. Herdado de [identityProviderBase](../resources/identityproviderbase.md). Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição exclusivo do provedor de identidade. Herdado de [identityProviderBase](../resources/identityproviderbase.md).|
|identityProviderType|Cadeia de caracteres|A identidade do provedor de identidade. Para um cenário B2B, valores possíveis: `AADSignup`, `MicrosoftAccount`, `EmailOTP`. Obrigatório.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.builtInIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "builtinIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
