---
title: Criar mailSearchFolder
description: Use esta API para criar um novo mailSearchFolder na caixa de correio do usuário especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bdebbcb9c842d57d4c6ee8d8eb72f45df74a22d7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333306"
---
# <a name="create-mailsearchfolder"></a>Criar mailSearchFolder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use esta API para criar um novo [mailSearchFolder](../resources/mailsearchfolder.md) na caixa de correio do usuário especificado.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Mail.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Mail.ReadWrite    |
|Aplicativo | Mail.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido. Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho | Valor |
|:-------|:------|
| Autorização | `Bearer {token}`. Obrigatório. |
| Content-Type | `application/json`. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro | Tipo | Descrição |
|:----------|:-----|:------------|
| @odata.type | String | O tipo de pasta a ser criada. Defina como "Microsoft. Graph. mailSearchFolder". |
| displayName | String | O nome de exibição da nova pasta.|
| includeNestedFolders | Boolean | Como a hierarquia da pasta de caixa de correio deve ser percorrida. `true`significa que uma pesquisa profunda deve ser feita enquanto `false` uma pesquisa superficial deve ser realizada. |
| sourceFolderIDs | Coleção String | As pastas de caixa de correio que devem ser minadas. |
| filterQuery | String | A consulta OData para filtrar as mensagens. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [mailSearchFolder](../resources/mailsearchfolder.md) no corpo da resposta.

## <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "create_mailsearchfolder"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childfolders
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "displayName": "Get MyAnalytics",
  "includeNestedFolders": true,
  "sourceFolderIDs": ["AAMkAGVmMDEzM"],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 13,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
    "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
