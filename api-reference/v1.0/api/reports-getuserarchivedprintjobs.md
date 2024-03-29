---
title: 'reports: getUserArchivedPrintJobs'
description: Obter uma lista de trabalhos de impressão arquivados para um usuário específico.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 50f48985beebb5230ece74fd62d6f793da364d6c
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863576"
---
# <a name="reportroot-getuserarchivedprintjobs"></a>reportRoot: getUserArchivedPrintJobs
Namespace: microsoft.graph

Obter uma lista de trabalhos de impressão arquivados para um usuário específico.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegada (conta corporativa ou de estudante)| Reports.Read.All |
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getUserArchivedPrintJobs
```

## <a name="function-parameters"></a>Parâmetros de função

Na URL de solicitação, forneça os seguintes parâmetros de função com valores:

| Parâmetro     | Tipo                 | Obrigatório? | Descrição                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `userId`      | `Edm.String`         | Sim       | A ID do usuário para o que retornar dados.                               |
| `startDateTime` | `Edm.DateTimeOffset` | Não        | A data de início (inclusive) do período de tempo a ser incluído.|
| `endDateTime`   | `Edm.DateTimeOffset` | Não        | A data de término (inclusive) do período de tempo a ser incluído.|

>**Observação:** Se um valor não for necessário, passe o parâmetro com valor nulo.
## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código `200 OK` de resposta e uma coleção [archivedPrintJob](../resources/archivedprintjob.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "reportroot_getuserarchivedprintjobs"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/getUserArchivedPrintJobs(userId='{id}',startDateTime=<timestamp>,endDateTime=<timestamp>)
```

### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.archivedPrintJob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "fe6ff85a-f0d3-4c4f-aec6-b9d5154356a1",
      "createdBy": {},
      "processingState": "completed"
    }
  ]
}
```

