---
title: Tipo de recurso permissionScope
description: Representa a definição de uma permissão delegada, às vezes referida como uma permissão OAuth 2.0 ou um escopo OAuth 2.0. Depois de definida, a permissão delegada pode ser solicitada por um aplicativo cliente
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 2ca5b717c44ac1d0652deeaba30dd9ddcd2e00f7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137638"
---
# <a name="permissionscope-resource-type"></a>Tipo de recurso permissionScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a definição de [uma permissão delegada.](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)

As permissões delegadas podem ser solicitadas por aplicativos cliente que precisam de um token de acesso para a API que definiu as permissões. As permissões delegadas podem [](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent)ser solicitadas dinamicamente, usando o parâmetro em uma solicitação de autorização para a Microsoft Identity Platform, ou estaticamente, por meio da coleção `scopes` **requiredResourceAccess** [](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope)no objeto de aplicativo. [](application.md)

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|adminConsentDescription|String|Uma descrição das permissões delegadas, destinada a ser lida por um administrador concedendo a permissão em nome de todos os usuários. Esse texto aparece nas experiências de consentimento de administrador em todo o locatário.|
|adminConsentDisplayName|String|O título da permissão, destinado a ser lido por um administrador que concede a permissão em nome de todos os usuários.|
|id|Guid|Identificador exclusivo de permissão delegada dentro da coleção de permissões delegadas definidas para um aplicativo de recurso.|
|isEnabled|Booliano|Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão). Para excluir uma permissão, essa propriedade deve primeiro ser definida como **false**.  Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.|
|type|String|Especifica se essa permissão delegada deve ser considerada segura para usuários não administradores concordarem em nome de si mesmos ou se um administrador deve ser obrigado a consentir com as permissões. Esse será o comportamento padrão, mas cada cliente pode optar por personalizar o comportamento em sua organização (permitindo, restringindo ou limitando o consentimento do usuário para essa permissão delegada.)|
|userConsentDescription|String|Uma descrição das permissões delegadas, destinada a ser lida por um usuário que concede a permissão em seu próprio nome. Esse texto aparece nas experiências de consentimento em que o usuário está consentindo apenas em nome de si mesmo.|
|userConsentDisplayName|String|Um título para a permissão, destinado a ser lido por um usuário que concede a permissão em seu próprio nome. Esse texto aparece nas experiências de consentimento em que o usuário está consentindo apenas em nome de si mesmo.|
|value|Cadeia de caracteres|Especifica o valor a ser incluído na declaração `scp` (escopo) nos tokens de acesso. Não deve exceder 120 caracteres de comprimento. Os caracteres `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` permitidos são , bem como caracteres nos intervalos `0-9` e `A-Z` `a-z` . Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "id": "guid",
  "adminConsentDisplayName": "string",
  "adminConsentDescription": "string",
  "userConsentDisplayName": "string",
  "userConsentDescription": "string",
  "value": "string",
  "type": "string",
  "isEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
