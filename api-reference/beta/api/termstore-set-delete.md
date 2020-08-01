---
title: Excluir conjunto
description: Excluir um objeto Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 83b48322c28330d22047a15cc488d276281fcc71
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539138"
---
# <a name="delete-set"></a>Excluir conjunto
Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Excluir um objeto [set](../resources/termstore-set.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante) |TermStore.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |


## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "delete_set"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}
```


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete termSet",
  "suppressions": [
  ]
}
-->
