---
author: JeremyKelley
description: Cria de forma assíncrona uma cópia de um [driveItem][item-resource] (incluindo qualquer filho), em um novo item pai ou com um novo nome.
ms.date: 09/10/2017
title: 'driveItem: copiar'
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 236d647414b42023a939ef7728e356091f59aa74
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/08/2022
ms.locfileid: "62443160"
---
# <a name="driveitem-copy"></a>driveItem: copiar

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Cria uma cópia de forma assíncrona de um [driveItem][item-resource] (incluindo os filhos), em um novo item pai ou com um novo nome.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All    |
|Aplicativo | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte ao `@microsoft.graph.conflictBehavior` parâmetro de consulta para personalizar o comportamento quando ocorre um conflito.

| Valor           | Descrição                                    |
|:----------------|:---------------------------------------------- |
| fail            | O comportamento padrão é relatar a falha.     |
| replace         | Substituir item existente no site de destino.    |
| rename          | Renomeie o item.                               |

**Observação:** O _conflictBehavior_ não é suportado para OneDrive Consumidor.

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.


| Nome            | Valor                                          | Descrição                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| parentReference | [ItemReference](../resources/itemreference.md) | Opcional. Referência ao item pai em que a cópia será criada.                                         |
| nome            | string                                         | Opcional. O novo nome para a cópia. Se isso não for fornecido, será usado o mesmo nome que o original.    |

**Observação:** _parentReference_ deve incluir os parâmetros `driveId` e `id` para a pasta de destino.

## <a name="response"></a>Resposta

Retorna detalhes sobre como [monitorar o progresso](/graph/long-running-actions-overview) da cópia após aceitar a solicitação.

## <a name="example"></a>Exemplo

Este exemplo copia um arquivo identificado por `{item-id}` em uma pasta identificada por um valor `driveId` e `id`.
A nova cópia do arquivo será nomeada `contoso plan (copy).txt`.

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/copy-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/copy-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/copy-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/copy-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
<!-- { "blockType": "response" } -->
```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```
O valor do cabeçalho `Location` fornece uma URL para um serviço que irá retornar o estado atual da operação de cópia.
Você pode usar essas informações [para determinar quando a cópia foi concluída](/graph/long-running-actions-overview).

### <a name="remarks"></a>Comentários

Em muitos casos, a ação de copiar é executada de forma assíncrona.
A resposta da API indicará apenas que a operação de cópia foi aceita ou rejeitada; por exemplo, devido ao nome do arquivo de destino já estar em uso.

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->


