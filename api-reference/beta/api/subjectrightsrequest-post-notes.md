---
title: Criar authoredNote
description: Crie um novo objeto AuthoredNote.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 811e0063b44e942aaeb13cf4069780b4635636d9
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60447015"
---
# <a name="create-authorednote"></a>Criar authoredNote
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto AuthoredNote.](../resources/authorednote.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|SubjectRightsRequest.ReadWrite.All*|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte|

>[!IMPORTANT]
>No momento, as permissões marcadas com um asterisco (*) não estão disponíveis. Para mais detalhes, confira [Problemas conhecidos](/graph/known-issues#compliance).

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto authoredNote.](../resources/authorednote.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [a authoredNote](../resources/authorednote.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|content|[microsoft.graph.itemBody](../resources/itembody.md)|O conteúdo da nota para a solicitação|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto authoredNote](../resources/authorednote.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_authorednote_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
Content-Type: application/json
Content-length: 203

{
"content": 
  {
    "content": "String",
    "contentType": "text"
  }
}
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authoredNote"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "String (identifier)",
    "createdDateTime": "String (timestamp)",
    "author": { "@odata.type": "microsoft.graph.identitySet"},
    "content": {
          "@odata.type": "microsoft.graph.itemBody"
    }

}
```

