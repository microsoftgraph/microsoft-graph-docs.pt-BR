---
title: tipo de recurso permissionScope
description: Representa a definição de uma permissão delegada, às vezes referida como uma permissão OAuth 2,0 ou um escopo de 2,0 OAuth. Uma vez definido, a permissão delegada pode ser solicitada por um aplicativo cliente
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 44919f6defadd4f5954d6b7a7959e0e0588371ba
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287014"
---
# <a name="permissionscope-resource-type"></a>tipo de recurso permissionScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a definição de uma [permissão delegada](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).

As permissões delegadas podem ser solicitadas por aplicativos cliente que precisam de um token de acesso para a API que definiu as permissões. As permissões delegadas podem ser solicitadas [dinamicamente](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), usando o `scopes` parâmetro em uma solicitação de autorização para a plataforma de identidade da Microsoft, ou [estaticamente](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope), através da coleção **requiredResourceAccess** no objeto [Application](application.md) .

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|adminConsentDescription|String|Uma descrição das permissões delegadas, que devem ser lidas por um administrador que concede a permissão em nome de todos os usuários. Esse texto aparece em experiências de consentimento de administrador em todo o locatário.|
|adminConsentDisplayName|String|O título da permissão, destinado a ser lido por um administrador que concede a permissão em nome de todos os usuários.|
|id|Guid|Identificador de permissão delegada exclusiva dentro da coleção de permissões delegadas definido para um aplicativo de recurso.|
|isEnabled|Boolean|Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão). Para excluir uma permissão, essa propriedade deve ser definida primeiro como **false**.  Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.|
|type|String|Especifica se essa permissão delegada deve ser considerada segura para que usuários que não são administradores consentissem em nome de si mesmas ou se um administrador deve ser necessário para o consentimento das permissões. Esse será o comportamento padrão, mas cada cliente poderá optar por personalizar o comportamento em sua organização (permitindo, restringindo ou limitando o consentimento do usuário a essa permissão delegada).|
|userConsentDescription|String|Uma descrição das permissões delegadas, que devem ser lidas por um usuário que concede a permissão em seu próprio nome. Esse texto aparece em experiências de consentimento onde o usuário está concordando somente em nome de si mesmo.|
|userConsentDisplayName|String|Um título para a permissão, que deve ser lido por um usuário que conceda a permissão em seu próprio nome. Esse texto aparece em experiências de consentimento onde o usuário está concordando somente em nome de si mesmo.|
|value|Cadeia de caracteres|Especifica o valor a ser incluído na `scp` declaração (escopo) em tokens de acesso. Não deve exceder 120 caracteres de comprimento. Os caracteres permitidos são `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` , bem como os caracteres nos intervalos `0-9` `A-Z` e `a-z` . Qualquer outro caractere, incluindo o caractere de espaço, não é permitido.|

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
