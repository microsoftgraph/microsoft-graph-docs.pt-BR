---
title: 'ediscoverySearch: estimateStatistics'
description: Executa uma estimativa da pesquisa de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 0809dbad83052bdd6a8de830df8cb522c61ba693
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839097"
---
# <a name="ediscoverysearch-estimatestatistics"></a>ediscoverySearch: estimateStatistics
Namespace: microsoft.graph.security

Execute uma estimativa do número de emails e documentos na pesquisa de Descoberta Eletrônica. Para saber mais sobre pesquisas na Descoberta Eletrônica, consulte Coletar dados para obter um caso na [Descoberta Eletrônica (Premium)](/microsoft-365/compliance/collecting-data-for-ediscovery).


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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/estimateStatistics
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se a estimativa for iniciada com êxito, essa ação retornará um código `202 Accepted` de resposta.
A resposta também conterá `Location` um cabeçalho, que contém o local do [microsoft.graph.security.estimateStatisticsOperation](../resources/security-ediscoveryestimateoperation.md) que foi criado para lidar com a estimativa. Verifique o status da operação de estimativa fazendo uma solicitação GET para o local.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "ediscoverysearchthis.estimatestatistics"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/estimatestatistics
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```