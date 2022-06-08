---
title: 'ediscoveryReviewSet: addToReviewSet'
description: Inicie o processo de adição de uma coleção de serviços do Microsoft 365 a um conjunto de revisão.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 8ae8a25bb90e647c4bd4795febf321a2a7208421
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945192"
---
# <a name="ediscoveryreviewset-addtoreviewset"></a>ediscoveryReviewSet: addToReviewSet
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Inicie o processo de adição de uma coleção de serviços do Microsoft 365 a um conjunto de revisão. Depois que a operação for criada, você poderá obter o status `Location` da operação recuperando o parâmetro dos cabeçalhos de resposta. O local fornece uma URL que retornará uma operação [Adicionar ao conjunto de revisão](../resources/security-ediscoveryaddtoreviewsetoperation.md).


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /ediscoveryExportOperation/reviewSet/addToReviewSet
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|search|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|A ID da pesquisa de Descoberta Eletrônica que você deseja adicionar ao conjunto de revisão.|
|additionalDataOptions|additionalDataOptions|As opções para adicionar itens ao reviewSet.|

### <a name="additionaldataoptions-values"></a>valores additionalDataOptions
|Nome|Descrição|
|:---|:---|
|allVersions|incluem todas as versões de um documento do SharePoint correspondentes à consulta de coleção de origem. Cuidado: as versões do SharePoint podem aumentar significativamente o volume de itens |
|linkedFiles|incluem arquivos vinculados que foram compartilhados no Outlook, equipes ou mensagens do Yammer anexando um link ao arquivo.|

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewsetthis.addtoreviewset"
}
-->
``` http
POST https://graph.microsoft.com/beta/ediscoveryExportOperation/reviewSet/addToReviewSet
Content-Type: application/json

{
    "search": {
        "id": "7c165312-d8db-48b5-9129-1af50932df53"
    },
    "additionalDataOptions": "linkedFiles"
}
```


### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```