---
author: JeremyKelley
title: Criar pacote
description: Criar um pacote de driveItems
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: dc6f1cf54cc615b65abe3573a9b6481f83a9f3be
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561594"
---
# <a name="create-bundle"></a>Criar pacote

Namespace: microsoft.graph

Adicione um novo [pacote][] à unidade do usuário.

[bundle]: ../resources/bundle.md

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte.                             |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All   |
|Aplicativo          | Sem suporte.                                           |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição  |
|:------------- |:------------ |
| Autorização | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do pacote a ser criado.

## <a name="response"></a>Resposta

Se a solicitação for bem-sucedida, [o driveItem](../resources/driveitem.md) que representa o pacote recém-criado será retornado.

Para obter informações sobre respostas de erro, consulte [Respostas de erro][error-response].

## <a name="examples"></a>Exemplos

### <a name="example-1-create-a-bundle"></a>Exemplo 1: Criar um pacote

O exemplo a seguir mostra como criar um novo pacote básico.
Essa solicitação criará um novo pacote chamado `Just some files` e adicionará dois itens existentes ao pacote.
Esse pacote pode ser usado para compartilhar uma coleção de arquivos com outros usuários sem compartilhar a pasta em que esses itens são armazenados.

#### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "name": "create-bundle" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "Just some files",
  "@microsoft.graph.conflictBehavior" : "rename",
  "bundle": { },
  "children": [
    { "id": "1234asdf" },
    { "id": "1234qwerty" }
  ]
}
```

#### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2
  }
}
```

O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.

### <a name="example-2-create-an-album"></a>Exemplo 2: Criar um álbum

A solicitação para criar um novo álbum de fotos é semelhante, embora dentro da faceta do pacote, a propriedade do álbum seja definida como um valor não nulo.

#### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "name": "create-album" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "My Day at the Beach",
  "@microsoft.graph.conflictBehavior" : "rename",
  "bundle": { "album": {} },
  "children": [
    { "id": "1234asdf" }
  ]
}
```

#### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2,
    "album": { }
 }
}
```

O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.

Se _@microsoft.graph.conflictBehavior_ estiver definido para **renomear** e um pacote com o mesmo nome já existir, o novo nome do pacote será atualizado para ser exclusivo.
OneDrive anexar um número ao final do nome do pacote.

Por exemplo, `My Day at the Beach` poderia ser renomeado `My Day at the Beach 1`.
Se `My Day at the Beach 1` for tomada, o número será incrementado novamente até que um nome de pacote exclusivo seja descoberto.


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Create"
} -->


