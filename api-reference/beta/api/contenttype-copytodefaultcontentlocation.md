---
author: swapnil1993
title: 'contentType: copyToDefaultContentLocation'
description: Copie um arquivo para um local de conteúdo padrão em um tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 913db69991d176d8537baef5abbbb8734d6c10cc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445879"
---
# <a name="contenttype-copytodefaultcontentlocation"></a>contentType: copyToDefaultContentLocation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Copie um arquivo para um local de conteúdo padrão em um [tipo de conteúdo][contentType]. Em seguida, o arquivo pode ser adicionado como um arquivo ou modelo padrão por meio de uma operação POST.

## <a name="permissions"></a>Permissões  

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).

  

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

```http

POST /sites/id/contentTypes/id/copyToDefaultContentLocation 
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.


|Parâmetro|Tipo|Descrição|
|-|-|-|
|sourceFile| [itemReference](../resources/itemreference.md) |Metadados sobre o arquivo de origem que precisa ser copiado para o local de conteúdo padrão. Obrigatório.|
|destinationFileName| string |Nome do arquivo de destino. 

## <a name="response"></a>Resposta


Se tiver êxito, essa chamada retornará uma `204 No Content` resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "contenttype_copytodefaultcontentlocation"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{id}/contentTypes/{contentTypeId}/copyToDefaultContentLocation 
Content-Type: application/json

{
    "sourceFile": {
        "sharepointIds": {
            "listId": "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0",
            "listItemId": "2"
        }
    },
    "destinationFileName": "newname.txt"
}
```



### <a name="response"></a>Resposta


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content

```

  

[contentType]: ../resources/contentType.md
