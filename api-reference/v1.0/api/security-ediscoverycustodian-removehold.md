---
title: 'ediscoveryCustodian: removeHold'
description: '**TODO: adicionar descrição**'
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 4069641d0079d450b6370d47167e6e49872f0f66
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839122"
---
# <a name="ediscoverycustodian-removehold"></a>ediscoveryCustodian: removeHold
Namespace: microsoft.graph.security

Inicie o processo de remoção da retenção dos [custodiantes da Descoberta Eletrônica](../resources/security-ediscoverycustodian.md). Depois que a operação for criada, você poderá obter o status recuperando `Location` o parâmetro dos cabeçalhos de resposta. O local fornece uma URL que retornará [um objeto eDiscoveryHoldOperation](../resources/security-ediscoveryholdoperation.md) .

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/removeHold
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/{eDiscoveryCustodianId}/removeHold
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
|ids|Coleção de cadeias de caracteres|As IDs dos custodiantes a serem aplicadas. Opcional.|


## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.

## <a name="examples"></a>Exemplos
### <a name="example-1-remove-hold-from-multiple-custodians"></a>Exemplo 1: remover a retenção de vários custodiantes
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "ediscoverycustodianthis.removehold"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/removeHold
Content-Type: application/json

{
  "ids": [
    "7f697316-43ed-48e1-977f-261be050db93", "b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8"
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

### <a name="example-2-remove-hold-from-a-single-custodian"></a>Exemplo 2: remover a retenção de um único guardião
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "ediscoverycustodianthis.removehold"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/c25c3914f9f743ee9cbaa25377e0cec6/removeHold
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