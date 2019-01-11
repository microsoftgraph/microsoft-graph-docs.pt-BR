---
title: tipo de recurso de permissionScope
description: Representa um OAuth 2.0 delegada escopo de permissão. O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de aplicativo) ao chamar um aplicativo de recurso. A propriedade **oauth2Permissions** da entidade ServicePrincipal e da entidade do aplicativo é uma coleção de **OAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: a294316f5c6255d0873ce0dbe809c33dad89ae08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818148"
---
# <a name="permissionscope-resource-type"></a>tipo de recurso de permissionScope

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um OAuth 2.0 delegada escopo de permissão. O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de [aplicativo](application.md) ) ao chamar um aplicativo de recurso. A propriedade **oauth2Permissions** da entidade [ServicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **OAuth2Permission**.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|adminConsentDescription|Cadeia de caracteres| Texto de ajuda de permissão que aparece nas experiências de atribuição de consentimento e app admin. |
|adminConsentDisplayName|Cadeia de caracteres| Nome para exibição da permissão que aparece nas experiências de atribuição de consentimento e app admin. |
|id|Guid| Identificador de permissão de escopo exclusiva dentro da coleção oauth2Permissions. |
|isEnabled|Boolean| Ao criar ou atualizar uma permissão, essa propriedade deverá ser definida como **true** (o que é o padrão). Para excluir uma permissão, essa propriedade primeiro deve ser definida como **false**. Nesse momento, em uma chamada subsequente, a permissão pode ser removida. |
|origem|Cadeia de caracteres| Para uso interno. |
|type|Cadeia de caracteres| Especifica se esta permissão de escopo pode ser consentiu por um usuário final, ou se é uma permissão de todo o inquilino deve ser consentiu por um administrador da empresa. Valores possíveis são o *usuário* ou *administrador*. |
|userConsentDescription|Cadeia de caracteres| Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final. |
|userConsentDisplayName|Cadeia de caracteres| Nome para exibição da permissão que aparece na experiência de consentimento do usuário final. |
|valor|Cadeia de caracteres| O valor da declaração escopo que deve esperar que o aplicativo de recurso no token de acesso OAuth 2.0. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
