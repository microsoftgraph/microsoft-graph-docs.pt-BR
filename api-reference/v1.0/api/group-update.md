---
title: Atualizar grupo
description: Atualizar as propriedades de um objeto group.
author: Jordanndahl
ms.localizationpriority: high
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 644470934cd334245375bdd8b76e3b11a4bd2099
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340722"
---
# <a name="update-group"></a>Atualizar grupo

Namespace: microsoft.graph

Atualizar as propriedades de um objeto group.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça *apenas* os valores das propriedades que devem ser atualizadas. As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base nas alterações em outros valores de propriedade.

A tabela a seguir especifica as propriedades que podem ser atualizadas.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean|O padrão é `false`. Indica se as pessoas externas à organização podem enviar mensagens ao grupo.|
|autoSubscribeNewMembers|Boolean|O padrão é `false`. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email. **autoSubscribeNewMembers** não pode ser `true` quando **subscriptionEnabled** é definido como `false` no grupo.|
|descrição|String|Uma descrição opcional para o grupo. |
|displayName|Cadeia de caracteres|O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. |
|mailNickname|String|O alias de email do grupo, exclusivo para grupos do Microsoft 365 na organização. O comprimento máximo é de 64 caracteres. Essa propriedade pode conter apenas caracteres no [conjunto de caracteres ASCII de 0 a 127](/office/vba/language/reference/user-interface-help/character-set-0127), exceto o seguinte: ` @ () \ [] " ; : . <> , SPACE`. |
|preferredDataLocation|String|O local de dados preferencial para o grupo Microsoft 365. Para atualizar essa propriedade, o usuário de chamada deve receber uma das seguintes funções do Azure Active Directory: <br><ul><li> Administrador Global <li> Administrador de Conta de Usuário <li> Suporte para Parceiro Nível1 ou Nível2 <li>Gravador de Diretório <li> Administrador do Exchange <li> Administrador do SharePoint </ul> <br/>Para obter mais informações sobre essa propriedade, consulte [OneDrive Online Multi-Geo](/sharepoint/dev/solution-guidance/multigeo-introduction).|
|securityEnabled|Boolean|Especifica se o grupo é um grupo de segurança. |
|visibility|Cadeia de caracteres|Especifica a visibilidade de um grupo do Microsoft 365. Os valores possíveis são: **Privado**, **Público** ou vazio (que é interpretado como **Público**).|

> [!IMPORTANT]
>
> + Para atualizar as seguintes propriedades, você deve especificá-las em sua própria solicitação PATCH, sem incluir as outras propriedades listadas na tabela acima: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.
>
> + Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers**, dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](/graph/known-issues#groups).
>
> + As regras para atualizar os grupos de segurança habilitados para email no Microsoft Exchange Server podem ser complexas; Para saber mais, confira [Gerenciar grupos de segurança habilitados para email no Exchange Server](/Exchange/recipients/mail-enabled-security-groups).

## <a name="response"></a>Resposta

Se for bem-sucedido, este método retorna um código de resposta `204 No Content`, exceto um código de resposta `200 OK` ao atualizar as seguintes propriedades: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como atualizar um grupo.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
Content-type: application/json

{
  "description": "Library Assist",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library-help"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
