---
title: Excluir teamsApp
description: 'Exclua Teams aplicativo do catálogo de aplicativos de uma organização (o catálogo de aplicativos de locatário). '
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cc1f678f6816ba6fb7ea3e91d244bf00d8a5edbf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109854"
---
# <a name="delete-teamsapp"></a>Excluir teamsApp

Namespace: microsoft.graph

<!-- markdownlint-disable MD001 -->
### <a name="delete-an-app-from-your-organizations-app-catalog"></a>Excluir um aplicativo do catálogo de aplicativos da sua organização

[Exclua um aplicativo](../resources/teamsapp.md) do catálogo de aplicativos de uma organização (o catálogo de aplicativos do locatário). Para excluir um aplicativo, a **propriedade distributionMethod** para o aplicativo deve ser definida como `organization` .

Você também pode usar essa API para remover um aplicativo enviado do processo de revisão.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Observação:** Somente administradores globais podem chamar essa API.

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)|
|:----------------------------------     |:-------------|
| Delegada (conta corporativa ou de estudante) | AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte|
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

Para excluir um aplicativo do catálogo de aplicativos:

<!-- { "blockType": "ignored" } -->
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
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
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

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

