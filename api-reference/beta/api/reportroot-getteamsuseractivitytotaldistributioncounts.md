---
title: 'reportRoot: getTeamsUserActivityTotalDistributionCounts'
description: Obtenha o número de atividades Microsoft Teams usuário durante o período selecionado. Os tipos de atividade são mensagens de chat de equipe, mensagens de chat privadas, chamadas, reuniões, reuniões organizadas, reuniões atendidas, duração do áudio, duração do vídeo, duração do compartilhamento de tela, mensagens de postagem e mensagens de resposta.
ms.localizationpriority: medium
ms.prod: reports
author: zhiliqiao
doc_type: apiPageType
ms.openlocfilehash: bfd2c37c542392022e0347089f0a1b4382265842
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704480"
---
# <a name="reportroot-getteamsuseractivitytotaldistributioncounts"></a>reportRoot: getTeamsUserActivityTotalDistributionCounts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha o número de atividades Microsoft Teams usuário durante o período selecionado. Os tipos de atividade são mensagens de chat de equipe, mensagens de chat privadas, chamadas, reuniões, reuniões organizadas, reuniões atendidas, duração do áudio, duração do vídeo, duração do compartilhamento de tela, mensagens de postagem e mensagens de resposta.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :--------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All                         |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                           |
| Aplicativo                            | Reports.Read.All                         |

> **Observação**: para permissões delegadas permitirem que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador Azure Active Directory limitada apropriada. Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityTotalDistributionCounts(period='{period_value}')
```

## <a name="function-parameters"></a>Parâmetros de função

Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.

| Parâmetro | Tipo   | Descrição                              |
| :-------- | :----- | :--------------------------------------- |
| ponto    | cadeia de caracteres | Especifica o período de tempo durante o qual o relatório é agregado. Os valores com suporte para {period_value} são: `D7`, `D30`, `D90`e `D180`. Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado. Obrigatório.|

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta. O tipo de saída padrão é `text/csv`. No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData `$format` para definir a saída padrão como `text/csv` ou `application/json`.

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
- Mensagens de chat de equipes
- Mensagens de chat privadas
- Chamadas
- Reuniões
- Reuniões Organizadas
- Reuniões atendidas
- Duração do áudio
- Duração do vídeo
- Duração do Compartilhamento de Tela
- Postar Mensagens
- Mensagens de Resposta
- Período de Relatório

### <a name="json"></a>JSON

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto JSON no corpo da resposta.

O tamanho de página padrão para essa solicitação é de 2.000 itens.

## <a name="examples"></a>Exemplos

### <a name="example-1-csv-output"></a>Exemplo 1: saída CSV

A seguir está um exemplo que gera CSV.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalDistributionCounts(period='D7')?$format=text/csv
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

Report Refresh Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Meetings Organized,Meetings Attended,Audio Duration,Video Duration,Screen Share Duration,Post Messages,Reply Messages,Report Period
```

### <a name="example-2-json-output"></a>Exemplo 2: saída JSON

A seguir está um exemplo que retorna JSON.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalDistributionCounts(period='D7')?$format=application/json
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
Content-Length: 661

{
  "@odata.context": "https://graph.microsoft.com/beta/getTeamsUserActivityTotalDistributionCounts(period='D7')?$format=application/json&$skiptoken=D07uj", 
  "value": [
      "reportRefreshDate": "2021-09-01", 
      "userCounts"
        {
          "reportPeriod":7,
          "teamChatMessages": 26, 
          "privateChatMessages": 17, 
          "calls": 4, 
          "meetings": 0, 
          "audioDuration": 00:00:00,
          "videoDuration": 00:00:00,
          "screenShareDuration": 00:00:00,
          "meetingsOrganized": 0,
          "meetingsAttended": 0,
          "postMessages": 1,
          "replyMessages": 1
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


