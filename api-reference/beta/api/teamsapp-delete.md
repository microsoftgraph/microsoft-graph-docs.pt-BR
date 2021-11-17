---
title: Excluir teamsApp
description: 'Remova um Teams do catálogo de aplicativos de uma organização (o catálogo de aplicativos de locatário). '
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5c98c7f5a81a3f7dfdf6a14bf799ae0a0852bdf8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977656"
---
# <a name="delete-teamsapp"></a>Excluir teamsApp

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD001 -->

[Exclua um aplicativo](../resources/teamsapp.md) do catálogo de aplicativos de uma organização (o catálogo de aplicativos do locatário). Para excluir um aplicativo, a **propriedade distributionMethod** para o aplicativo deve ser definida como `organization` .

Você também pode usar essa API para remover um aplicativo enviado do processo de revisão.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Observação:** Somente administradores globais podem chamar essa API. 

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)|
|:----------------------------------     |:-------------|
| Delegado (conta corporativa ou de estudante) | AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All** |
| Delegado (conta pessoal da Microsoft) | Sem suporte.|
| Aplicativo                            | Sem suporte. |

> **Observação**: as permissões marcadas com ** foram preteridas e não devem ser usadas.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

Para excluir um aplicativo do catálogo de aplicativos:

```http
DELETE /appCatalogs/teamsApps/{id}
```

Para excluir um aplicativo que foi enviado, mas não foi aprovado:

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

>**Observação:** Use a ID retornada da chamada Lista [de](./appcatalogs-list-teamsapps.md) aplicativos publicados para fazer referência ao aplicativo que você gostaria de excluir. Não use a ID do manifesto do pacote do aplicativo zip.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-teamsapp-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
