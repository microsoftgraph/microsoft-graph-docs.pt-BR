---
title: tipo de recurso appRole
description: Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja chamando outro aplicativo ou que possa ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada. A propriedade **appRoles** da entidade servicePrincipalName e da entidade Application é uma coleção de **appRole**.
localization_priority: Normal
ms.openlocfilehash: 4043d600bd19c61156cccd72f0d4e4f2e8352640
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778674"
---
# <a name="approle-resource-type"></a>tipo de recurso appRole

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma função de aplicativo que pode ser solicitada por um aplicativo cliente que esteja chamando outro aplicativo ou que possa ser usada para atribuir um aplicativo a usuários ou grupos em uma função de aplicativo especificada. A propriedade **appRoles** da entidade [servicePrincipalName](serviceprincipal.md) e da entidade [Application](application.md) é uma coleção de **appRole**.

> Importante: essa funcionalidade está desabilitada na versão atual.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRole"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowedMemberTypes|Coleção de cadeias de caracteres|Especifica se essa definição de função de aplicativo pode ser atribuída a usuários e grupos por meio da configuração de "usuário" ou a outros aplicativos (que estão acessando esse aplicativo em cenários de serviço de daemon) definindo como "aplicativo" ou ambos.|
|descrição|String|Texto de ajuda de permissão que aparece nas experiências de consentimento e atribuição de aplicativo de administração.|
|displayName|String|Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.|
|id|Guid|Identificador de função exclusivo dentro da coleção **appRoles** . Ao criar uma nova função de aplicativo, um novo identificador GUID deve ser fornecido. |
|isEnabled|Boolean|Ao criar ou atualizar uma função de aplicativo, isso deve ser definido como **true** (que é o padrão). Para excluir uma função, é necessário primeiro defini-la como **false**.  Nesse ponto, em uma chamada subsequente, essa função pode ser removida.|
|tenham|String| Somente leitura. Especifica se a função de aplicativo é definida no objeto Application ou no objeto servicePrincipalName. _Não_ deve ser incluído em solicitações POST ou patch. |
|value|Cadeia de caracteres|Especifica o valor que será incluído na `roles` declaração em tokens de autenticação e de acesso. Não deve exceder 120 caracteres de comprimento. Caracteres `:` `!` `#` `$` permitidos são `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `A-Z` como os caracteres nos intervalos `a-z`e. `0-9` `^` `@` `[` `]` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.  |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
