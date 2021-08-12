---
title: Tipo de recurso permissionScope
description: Representa a definição de uma permissão delegada, às vezes conhecida como uma permissão OAuth 2.0 ou um escopo OAuth 2.0. Depois de definida, a permissão delegada poderá ser solicitada por um aplicativo cliente
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 7836685c65fddd2d35a2d9bc47493bf2f240e51653ef8a264ac868be83b02e80
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196933"
---
# <a name="permissionscope-resource-type"></a>Tipo de recurso permissionScope

Namespace: microsoft.graph

Representa a definição de uma [permissão delegada](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).

As permissões delegadas podem ser solicitadas por aplicativos cliente que precisam de um token de acesso à API que definiu as permissões. As permissões delegadas podem ser solicitadas [dinamicamente](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), usando o parâmetro em uma solicitação de autorização para o plataforma de identidade da Microsoft, ou estaticamente, por meio da coleção `scopes` **requiredResourceAccess** no objeto [application.](application.md) [](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope)

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|adminConsentDescription|String|Uma descrição das permissões delegadas, destinadas a ser lidas por um administrador concedendo a permissão em nome de todos os usuários. Este texto aparece em experiências de consentimento de administrador em todo o locatário.|
|adminConsentDisplayName|Cadeia de caracteres|O título da permissão, destinado a ser lido por um administrador concedendo a permissão em nome de todos os usuários.|
|id|Guid|Identificador de permissão delegado exclusivo dentro da coleção de permissões delegadas definidas para um aplicativo de recurso.|
|isEnabled|Booliano|Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão). Para excluir uma permissão, essa propriedade deve primeiro ser definida como **false**.  Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.|
|tipo|Cadeia de caracteres|Especifica se essa permissão delegada deve ser considerada segura para usuários que não sejam administradores consentirem em nome de si mesmos ou se um administrador deve ser necessário para consentir as permissões. Esse será o comportamento padrão, mas cada cliente pode optar por personalizar o comportamento em sua organização (permitindo, restringindo ou limitando o consentimento do usuário para essa permissão delegada.)|
|userConsentDescription|String|Uma descrição das permissões delegadas, destinadas a ser lidas por um usuário concedendo a permissão em seu próprio nome. Este texto aparece em experiências de consentimento em que o usuário está consentindo apenas em nome de si mesmo.|
|userConsentDisplayName|Cadeia de caracteres|Um título para a permissão, destinado a ser lido por um usuário concedendo a permissão em seu próprio nome. Este texto aparece em experiências de consentimento em que o usuário está consentindo apenas em nome de si mesmo.|
|value|Cadeia de caracteres|Especifica o valor a ser incluído na declaração `scp` (escopo) em tokens de acesso. Não deve exceder 120 caracteres de comprimento. Os caracteres `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` permitidos são , bem como caracteres nos intervalos `0-9` `A-Z` e `a-z` . Qualquer outro caractere, incluindo o caractere de espaço, não é permitido. Pode não começar com `.` .|

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
