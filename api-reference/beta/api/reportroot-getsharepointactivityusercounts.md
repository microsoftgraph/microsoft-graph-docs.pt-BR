---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e3c806c991375d140a07c1fa09e19493f9b41f5b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513435"
---
# <a name="reportroot-getsharepointactivityusercounts"></a>reportRoot: getSharePointActivityUserCounts

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :--------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All                         |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                           |
| Aplicativo                            | Reports.Read.All                         |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a>Parâmetros de função

Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.

| Parâmetro | Tipo   | Descrição                              |
| :-------- | :----- | :--------------------------------------- |
| ponto    | string | Especifica o período de tempo durante o qual o relatório é agregado. Os valores com suporte para {period_value} são: D7, D30, D90 e D180. Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado. Obrigatório. |

Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta. O tipo de saída padrão é texto/csv. No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="response"></a>Resposta

### <a name="csv"></a>CSV

Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório. Essa URL pode ser encontrada no cabeçalho `Location` na resposta.

As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.

O arquivo CSV possui os seguintes cabeçalhos para colunas.

- Data de atualização do relatório
- Página visitada
- Exibidos ou editados
- Sincronizados
- Compartilhados internamente
- Compartilhados externamente
- Data do relatório
- Período de Relatório

### <a name="json"></a>JSON

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="csv"></a>CSV

O exemplo a seguir é um exemplo que emite CSV.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- { "blockType": "ignored" } --> 

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

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a>JSON

O exemplo a seguir é um exemplo que retorne JSON.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
