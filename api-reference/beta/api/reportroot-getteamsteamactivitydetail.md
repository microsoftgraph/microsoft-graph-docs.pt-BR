---
title: 'reportRoot: getTeamsTeamActivityDetail'
description: Obtenha detalhes sobre Microsoft Teams atividade por equipe. Os números incluem atividades para usuários licenciados e não licenciados.
ms.localizationpriority: medium
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7acd09947d4c37eb803f14cdc0cff508fac60172
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917810"
---
# <a name="reportroot-getteamsteamactivitydetail"></a>reportRoot: getTeamsTeamActivityDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha detalhes sobre Microsoft Teams atividade por equipe. Os números incluem atividades para usuários licenciados e não licenciados.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :--------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All                         |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                           |
| Aplicativo                            | Reports.Read.All                         |

> **Nota:** Para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador Azure Active Directory limitada apropriada. Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsTeamActivityDetail(period='{period_value}')
```

## <a name="function-parameters"></a>Parâmetros de função

Na URL da solicitação, forneça os parâmetros a seguir com um valor válido.

| Parâmetro | Tipo   | Descrição                              |
| :-------- | :----- | :--------------------------------------- |
| ponto    | cadeia de caracteres | Especifica o período de tempo durante o qual o relatório é agregado. Os valores com suporte para {period_value} são: `D7`, `D30`, `D90`e `D180`. Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado. Obrigatório. |
| data      | Data   | Especifica a data para a qual você deseja exibir detalhes sobre as atividades em uma ou mais equipes. {date_value} deve ter um formato de AAAA-MM-DD. Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo. |

> **Nota:** Você precisa definir o período **ou** a **data** na URL da solicitação.

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta. O tipo de saída padrão é `text/csv`. No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData `$format` para definir a saída padrão como `text/csv` ou `application/json`.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="response"></a>Resposta

### <a name="csv"></a>CSV

Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório. Essa URL pode ser encontrada no cabeçalho `Location` na resposta.

As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.

O arquivo CSV possui os seguintes cabeçalhos para colunas:

- Data de atualização do relatório
- Nome da Equipe
- ID da equipe
- Tipo de equipe
- Data da última atividade
- Período de Relatório
- Usuários ativos
- Canais ativos
- Convidados
- Reações
- Reuniões Organizadas
- Postar Mensagens
- Mensagens de Resposta
- Mensagens de canal
- Mensagens urgentes
- Menciona
- Canais Compartilhados Ativos
- Usuários Externos Ativos

### <a name="json"></a>JSON

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto JSON no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-csv-output"></a>Exemplo 1: saída CSV

A seguir está um exemplo que gera CSV.

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsTeamActivityDetail(period='D7')?$format=text/csv
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

Report Refresh Date,Team Name,Team Id,Team Type,Last Activity Date,Report Period,Active Users,Active Channels,Guests,Reactions,Meetings Organized,Post Messages,Reply Messages,Channel Messages,Urgent Messages,Mentions,Active Shared Channels,Active External Users
```

### <a name="example-2-json-output"></a>Exemplo 2: saída JSON

A seguir está um exemplo que retorna JSON.

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsTeamActivityDetail(period='D7')?$format=application/json
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
Content-Length: 876

{
  "@odata.context": "https://graph.microsoft.com/beta/reports/getTeamsTeamActivityDetail(period='D7')?$format=application/json&$skiptoken=D07uj", 
  "value": [
    {
      "reportRefreshDate": "2021-09-01", 
      "teamName": "sampleTeam",
      "teamId": "a063d832-ae9a-467d-8cb4-17c073260890",
      "teamType": "Private",
      "lastActivityDate": "2021-09-01",
      "details": [
        {
          "reportPeriod":7,
          "activeUsers": 26, 
          "activeChannels": 17, 
          "guests": 4, 
          "reactions": 36, 
          "meetingsOrganized": 0,
          "postMessages": 0,
          "replyMessages": 0,
          "channelMessages": 0,
          "urgentMessages": 0,
          "mentions": 0,
          "activeSharedChannels": "6",
          "activeExternalUsers": "8"
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
