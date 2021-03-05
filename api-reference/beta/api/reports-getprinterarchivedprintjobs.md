---
title: 'reports: getPrinterArchivedPrintJobs'
description: Obter uma lista de trabalhos de impressão arquivados que foram enluados para uma impressora específica.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: daf0acf2ab9bc285d05aae9f3b875ffc6f329b03
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472399"
---
# <a name="reports-getprinterarchivedprintjobs"></a>reports: getPrinterArchivedPrintJobs

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista de trabalhos de impressão arquivados que foram enluados para uma impressora [específica.](../resources/printer.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegada (conta corporativa ou de estudante)| Reports.Read.All |
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="function-parameters"></a>Parâmetros de função

| Parâmetro     | Tipo                 | Obrigatório? | Descrição                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | Sim       | A ID da impressora para a que retornar dados.                            |
| `startDateTime` | `Edm.DateTimeOffset` | Não        | A data de início (inclusive) do período de tempo a ser incluído. |
| `endDateTime`   | `Edm.DateTimeOffset` | Não        | A data de término (inclusive) do período de tempo a ser incluído.   |

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [archivedPrintJob](../resources/archivedprintjob.md) no corpo da resposta.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.
##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "reports-getprinterarchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getPrinterArchivedPrintJobs(printerId='{id}',startDateTime={timestamp},endDateTime={timestamp})
```

##### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.archivedPrintJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 236

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printer": {
        "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6"
      },
      "createdBy": {},
      "processingState": "completed"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: getPrinterArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

