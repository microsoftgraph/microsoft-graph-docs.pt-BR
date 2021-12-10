---
title: Tipo de recurso permissionScope
description: Representa a definição de uma permissão delegada, às vezes conhecida como uma permissão OAuth 2.0 ou um escopo OAuth 2.0. Depois de definida, a permissão delegada poderá ser solicitada por um aplicativo cliente
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 362bc29c76689993d016d5fb2f3efbfcfac7a54c
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2021
ms.locfileid: "61402857"
---
# <a name="permissionscope-resource-type"></a>Tipo de recurso permissionScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a definição de uma [permissão delegada](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).

As permissões delegadas podem ser solicitadas por aplicativos cliente que precisam de um token de acesso à API que definiu as permissões. As permissões delegadas podem ser solicitadas [dinamicamente](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), usando o parâmetro em uma solicitação de autorização para o plataforma de identidade da Microsoft, ou estaticamente, por meio da coleção `scopes` **requiredResourceAccess** no objeto [application.](application.md) [](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope)

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|adminConsentDescription|String|Uma descrição das permissões delegadas, destinadas a ser lidas por um administrador concedendo a permissão em nome de todos os usuários. Este texto aparece em experiências de consentimento de administrador em todo o locatário.|
|adminConsentDisplayName|String|O título da permissão, destinado a ser lido por um administrador concedendo a permissão em nome de todos os usuários.|
|id|Guid|Identificador de permissão delegado exclusivo dentro da coleção de permissões delegadas definidas para um aplicativo de recurso.|
|isEnabled|Booliano|Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão). Para excluir uma permissão, essa propriedade deve primeiro ser definida como **false**.  Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.|
|type|String| Os valores possíveis são: `User` e `Admin` . Especifica se essa permissão delegada deve ser considerada segura para que usuários não administradores consentam em nome de si mesmos ou se um consentimento de administrador sempre deve ser necessário. Embora o Microsoft Graph define o requisito de consentimento padrão para cada permissão, o administrador de locatários pode substituir o comportamento em sua organização (permitindo, restringindo ou limitando o consentimento do usuário para essa permissão delegada). Para obter mais informações, consulte [Configure how users consent to applications](/azure/active-directory/manage-apps/configure-user-consent). |
|userConsentDescription|String|Uma descrição das permissões delegadas, destinadas a ser lidas por um usuário concedendo a permissão em seu próprio nome. Este texto aparece em experiências de consentimento em que o usuário está consentindo apenas em nome de si mesmo.|
|userConsentDisplayName|String|Um título para a permissão, destinado a ser lido por um usuário concedendo a permissão em seu próprio nome. Este texto aparece em experiências de consentimento em que o usuário está consentindo apenas em nome de si mesmo.|
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
