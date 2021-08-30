---
author: swapnil1993
title: 'contentType: copyToDefaultContentLocation'
description: Copie um arquivo para um local de conteúdo padrão em um tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 4ca64f9a29b1471815784d10d0e23ec14c6a08fd
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696447"
---
# <a name="contenttype-copytodefaultcontentlocation"></a>contentType: copyToDefaultContentLocation
Namespace: microsoft.graph


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
POST /sites/{siteId}/contentTypes/{contentTypeId}/copyToDefaultContentLocation 
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
|destinationFileName| string |Nome do arquivo de destino. |

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
POST https://graph.microsoft.com/v1.0/sites/{siteId}/contentTypes/{contentTypeId}/copyToDefaultContentLocation 
Content-Type: application/json

{
   "sourceFile":{
      "sharepointIds":{
         "listId":"e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0",
         "listItemId":"2"
      }
   },
   "destinationFileName":"newname.txt"
}
```

### <a name="response"></a>Resposta


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

  

[contentType]: ../resources/contentType.md
