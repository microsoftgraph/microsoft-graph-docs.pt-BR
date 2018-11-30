---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Obter permissões
ms.openlocfilehash: 1964d291b6243ac286d5ac08a6bc48f3e576bbd3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040848"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a>Obter permissão de compartilhamento para um arquivo ou pasta

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Retornar a permissão de compartilhamento eficaz de um recurso de permissão específico.

Permissões efetivas de um item podem vir de duas fontes: permissões definidas diretamente no próprio item, ou permissões herdadas de ancestrais do item.

Os chamadores podem diferenciar se a permissão é herdada ou não verificando a propriedade `inheritedFrom` Esta propriedade é um recurso [itemReference](../resources/itemreference.md) que faz referência ao ancestral do qual a permissão é herdada.

Níveis de permissão do SharePoint definidos em um item retornam com um prefixo 'SP'. Por exemplo, SP.Somente exibição, SP.Acesso limitado, SP.Exibir Dados do Web Analytics. Consulte a [Lista completa de funções do SharePoint](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Aplicativo | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método é compatível com o [parâmetro de consulta $select](/graph/query-parameters) para formar a resposta.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [Permission](../resources/permission.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação para acessar uma permissão em uma pasta.

<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
```
### <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um recurso [Permission](../resources/permission.md) para a ID especificada. 

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a>Comentários

O recurso [Permission](../resources/permission.md) usa _facets_ para fornecer informações sobre o tipo de permissão representado pelo recurso.

Permissões com uma faceta [**link**](../resources/sharinglink.md) representam links de compartilhamento criados no item. Os links de compartilhamento contêm um token exclusivo que fornece acesso ao item para qualquer pessoa com o link.

Permissões com uma faceta [**invitation**](../resources/sharinginvitation.md) representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission"
}-->
