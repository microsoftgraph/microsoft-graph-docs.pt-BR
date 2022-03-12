---
title: Obter agreementFile
description: 'Recupere os detalhes do arquivo padrão para um contrato, incluindo as informações de idioma e versão. '
author: raprakasMSFT
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 20f4ea620ddb4b3031d854501d53c14d3a6cf461
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451521"
---
# <a name="get-agreementfile"></a>Obter agreementFile
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere os detalhes do arquivo padrão para um contrato, incluindo as informações de idioma e versão. As informações do arquivo são especificadas por meio do [objeto agreementFile](../resources/agreementfile.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Agreement.Read.All, Agreement.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /agreements/{agreementsId}/file
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção [de objetos agreementFile](../resources/agreementfile.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get_agreementfile"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/94410bbf-3d3e-4683-8149-f034e55c39dd/file
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementFile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/termsOfUse/agreements('94410bbf-3d3e-4683-8149-f034e55c39dd')/file/$entity",
    "@odata.type": "#microsoft.graph.agreementFileLocalization",
    "id": "08033369-8972-42a3-8533-90bbd2757a01",
    "fileName": "TOU.pdf",
    "displayName": "Contoso ToU for guest users",
    "language": "en",
    "isDefault": true,
    "isMajorVersion": false,
    "createdDateTime": "2022-03-04T13:14:13.9361722Z",
    "fileData": null
}
```

