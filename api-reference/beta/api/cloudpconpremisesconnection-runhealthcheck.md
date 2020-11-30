---
title: CloudPcOnPremisesConnection-RunHealthChecks
description: Executar verificações de integridade na conexão local do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 484d48f0400c328090d66bbcf7a930a485a9d950
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378209"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a>CloudPcOnPremisesConnection: runHealthChecks

Namespace: microsoft.graph

Executar verificações de integridade no objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .

Isso disparará uma nova verificação de integridade para este objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) e alterará as propriedades HealthCheckStatus e [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) quando o check for concluído.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
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
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
