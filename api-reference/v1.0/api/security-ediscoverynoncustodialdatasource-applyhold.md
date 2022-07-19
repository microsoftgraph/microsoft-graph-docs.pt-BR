---
title: 'ediscoveryNoncustodialDataSource: applyHold'
description: Inicie o processo de aplicação de retenção a fontes de dados não custodiais da Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 9c501b2586b7c4e1d34823859136961802d8fa7d
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839127"
---
# <a name="ediscoverynoncustodialdatasource-applyhold"></a>ediscoveryNoncustodialDataSource: applyHold
Namespace: microsoft.graph.security


Inicie o processo de aplicação de retenção em fontes de dados não [custodiais da Descoberta Eletrônica](../resources/security-ediscoverynoncustodialdatasource.md). Depois que a operação for criada, você poderá obter o status recuperando `Location` o parâmetro dos cabeçalhos de resposta. O local fornece uma URL que retornará [um objeto eDiscoveryHoldOperation](../resources/security-ediscoveryholdoperation.md) .

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources/applyHold
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources/{ediscoverynoncustodialDatasourceId}/applyHold
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
|ids|Coleção de cadeias de caracteres|As IDs de fontes de dados não custodiais a serem aplicadas à retenção. Opcional.|


## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.

## <a name="examples"></a>Exemplos

### <a name="example-1-apply-hold-to-multiple-non-custodial-data-sources"></a>Exemplo 1: Aplicar retenção a várias fontes de dados não custodiais
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "ediscoverynoncustialdatasource.applyhold"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/applyHold
Content-Type: application/json

{
    "ids": [
        "39333641443238353535383731453339",
        "46333131344239353834433430454335"
    ]
}
```


#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

### <a name="example-2-apply-hold-to-a-single-non-custodial-data-source"></a>Exemplo 2: Aplicar retenção a uma única fonte de dados não custodiante
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "ediscoverynoncustialdatasource.applyhold"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/39333641443238353535383731453339/applyHold
```


#### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
