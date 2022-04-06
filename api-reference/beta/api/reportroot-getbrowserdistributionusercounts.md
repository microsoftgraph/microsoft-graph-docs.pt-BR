---
title: 'reportRoot: getBrowserDistributionUserCounts'
description: Obter um relatório que fornece o número total de usuários usando Microsoft Edge, Versão Prévia do Microsoft Edge e o Internet Explorer quando usado para acessar os serviços Microsoft 365 por um período selecionado.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 171a17d29e37a0c8c560b5a643058fbb41f6c281
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589559"
---
# <a name="reportroot-getbrowserdistributionusercounts"></a>reportRoot: getBrowserDistributionUserCounts

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter um relatório que fornece o número total de usuários usando Microsoft Edge, Versão Prévia do Microsoft Edge e o Internet Explorer quando usado para acessar os serviços Microsoft 365 por um período selecionado.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 Relatórios no centro de administração - uso do navegador da Microsoft](/microsoft-365/admin/activity-reports/browser-usage-report).

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| -------------------------------------- | ------------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All                            |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Reports.Read.All                            |

> **Observação:** Para permissões delegadas permitirem que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador de locatários deve ter atribuído ao usuário a função de administrador Azure Active Directory limitada. Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getBrowserDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a>Parâmetros de função

Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.

| Parâmetro | Tipo   | Descrição                                                                                                                                                                                                                                                       |
| :-------- | :----- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ponto    | cadeia de caracteres | Especifica o período de tempo durante o qual o relatório é agregado. Os valores com suporte para {period_value} são: `D7`, `D30`, e `D90``D180`. Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado. Obrigatório. |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta. O tipo de saída padrão é `text/csv`. No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData `$format` para definir a saída padrão como `text/csv` ou `application/json`.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

### <a name="csv"></a>CSV

Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório. Essa URL pode ser encontrada no cabeçalho `Location` na resposta.

As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.

O arquivo CSV possui os seguintes cabeçalhos para colunas:

- Data de atualização do relatório
- Período de Relatório
- Borda
- Edge Legacy
- Internet Explorer

### <a name="json"></a>JSON

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto JSON no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-csv-output"></a>Exemplo 1: saída CSV

A seguir, um exemplo que dá saída ao CSV.

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getbrowserdistributionusercounts_csv"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getBrowserDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date, Report Period, Edge, Edge Legacy, Internet Explorer
```

### <a name="example-2-json-output"></a>Exemplo 2: saída JSON

A seguir, um exemplo que retorna JSON.

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getbrowserdistributionusercounts_json"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getBrowserDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
   "value":[
      {
         "reportRefreshDate":"2021-04-17",
         "userCounts":[
            {
               "reportPeriod":7,
               "edge":1269,
               "edgeLegacy":114,
               "ie":393
            },
            {
               "reportPeriod":30,
               "edge":1405,
               "edgeLegacy":383,
               "ie":708
            },
            {
               "reportPeriod":90,
               "edge":1482,
               "edgeLegacy":687,
               "ie":988
            },
            {
               "reportPeriod":180,
               "edge":1526,
               "edgeLegacy":860,
               "ie":1137
            }
         ]
      }
   ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
