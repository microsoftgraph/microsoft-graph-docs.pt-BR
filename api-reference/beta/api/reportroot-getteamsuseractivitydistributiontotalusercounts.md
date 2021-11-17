---
title: 'reportRoot: getTeamsUserActivityDistributionTotalUserCounts'
description: Obter o número de usuários Microsoft Teams licenciados ou não licenciados por tipo de atividade durante o período selecionado. Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões.
ms.localizationpriority: medium
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 87ad4531884b26d9ad598aafa8117827fceb915f
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044726"
---
# <a name="reportroot-getteamsuseractivitydistributiontotalusercounts"></a>reportRoot: getTeamsUserActivityDistributionTotalUserCounts

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o número de usuários Microsoft Teams licenciados ou não licenciados por tipo de atividade durante o período selecionado. Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :--------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All                         |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                           |
| Aplicativo                            | Reports.Read.All                         |

>**Observação**: para as permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador de locatários deve ter atribuído ao usuário a função de administrador limitada apropriada do Azure AD. Para obter mais detalhes, consulte [Autorização para as APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityDistributionTotalUserCounts(period='D7')
```

## <a name="function-parameters"></a>Parâmetros de função

Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.

| Parâmetro | Tipo   | Descrição                              |
| :-------- | :----- | :--------------------------------------- |
| ponto    | cadeia de caracteres | Especifica o período de tempo durante o qual o relatório é agregado. Os valores com suporte para {period_value} são: D7, D30, D90 e D180. Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado. Obrigatório. |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta. O tipo de saída padrão é text/csv. No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData definido como `$format` text/csv ou application/json.

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
- Mensagens de chat de equipes
- Mensagens de chat privadas
- Chamadas
- Reuniões
- Período de Relatório

### <a name="json"></a>JSON

Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto JSON no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="csv"></a>CSV

A seguir, um exemplo que dá saída ao CSV.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitydistributiontotalusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityDistributionTotalUserCounts(period='D7')?$format=text/csv
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

Report Refresh Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a>JSON

A seguir, um exemplo que retorna JSON.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitydistributiontotalusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityDistributionTotalUserCounts(period='D7')?$format=application/json
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
Content-Length: 291

{
  "value": [
    {
      "reportRefreshDate": "2020-09-01", 
      "teamChatMessages": 0, 
      "privateChatMessages": 0, 
      "calls": 0, 
      "meetings": 0, 
      "reportPeriod": "7"
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


