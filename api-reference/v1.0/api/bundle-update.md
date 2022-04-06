---
author: JeremyKelley
title: Atualizar um pacote
description: Atualizar um pacote de driveItems
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b4925016b63569bba1915ce83100f59e647acc1e
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561577"
---
# <a name="update-bundle"></a>Pacote de atualizações

Namespace: microsoft.graph

Atualize os metadados [para][] um [pacote de driveItemsdriveItem][] por ID.
Você só pode atualizar os seguintes metadados:

* Nome do pacote
* Album `coverImageItemId` (se aplicável)

Quaisquer outras solicitações de alteração serão ignoradas.

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
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição  |
|:------------- |:------------ |
| Autorização | \{token\} de portador. Obrigatório. |
| if-match      | eTag. Opcional. Se esse header de solicitação estiver incluído e a eTag fornecida não corresponder à eTag atual no buncle, uma `412 Precondition Failed` resposta será retornada.

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um [recurso driveItem][] que representa o pacote atualizado no corpo da resposta.

Para obter informações sobre respostas de erro, consulte [Respostas de erro][error-response].

## <a name="example"></a>Exemplo

Este exemplo renomeia um pacote.

### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "name": "rename-bundle" } -->

```http
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```

### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "Shared legal agreements",
  "bundle": {
    "childCount": 3
  }
}
```

O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of a bundle.",
  "keywords": "update,replace,contents,bundle",
  "section": "documentation",
    "tocPath&quot;: &quot;Bundles/Update"
} -->


