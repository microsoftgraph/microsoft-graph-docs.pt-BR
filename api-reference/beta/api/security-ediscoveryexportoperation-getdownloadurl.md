---
title: 'ediscoveryExportOperation: getDownloadUrl'
description: retornar um downloadUrl de onde o conteúdo de exportação é entregue como um fluxo
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7a990c67b5b444bc1d6b7db04c6e2035763e6363
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838091"
---
# <a name="ediscoveryexportoperation-getdownloadurl"></a>ediscoveryExportOperation: getDownloadUrl
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Se uma URL de blob do Azure não for fornecida na ação de exportação, a operação de exportação exportará os arquivos para um repositório interno. O conteúdo desse repositório pode ser buscado chamando essa função. Isso retornará um downloadUrl em que o conteúdo compactado é entregue como um fluxo.


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/operations/{eDiscoveryCaseOperationId}/microsoft.graph.security.ediscoveryExportOperation/getDownloadUrl
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código `200 OK` de resposta e uma cadeia de caracteres no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "ediscoveryexportoperationthis.getdownloadurl"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/ediscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/operations/c5ae226f457547a582ef0eb6dbfaee25/microsoft.graph.security.ediscoveryExportOperation/getDownloadUrl
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.String"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: text/plain

{
    "https://sdfpkgg0021.blob.edproxy.aed01.ediscovery.outlook.com/packaging120g37c10016472cb0abf28fac5800b0/6dec1a1c-0577-424f-819c-9542edc47f5a.zip?{SASToken}"
}
```

