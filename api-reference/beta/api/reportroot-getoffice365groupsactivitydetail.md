---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3d99cd7c80dd16c6ded518f7e1cbe9fecd0b3230
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515444"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a>reportRoot: getOffice365GroupsActivityDetail

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

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
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a>Parâmetros de função

Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.

| Parâmetro | Tipo   | Descrição                              |
| :-------- | :----- | :--------------------------------------- |
| ponto    | string | Especifica o período de tempo durante o qual o relatório é agregado. Os valores com suporte para {period_value} são: D7, D30, D90 e D180. Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado. |
| data      | Data   | Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade. {date_value} deve ter um formato de AAAA-MM-DD. Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo. |

> **Observação:** você precisa definir o período ou data na URL.

Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta. O tipo de saída padrão é texto/csv. No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.

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
- Nome de exibição do grupo
- Excluído
- Nome principal do proprietário
- Data da última atividade
- Tipo de grupo
- Contagem de Membros
- Contagem de membros externos
- Contagem de emails recebidos do Exchange
- Contagem de arquivos ativos do SharePoint
- Contagem de mensagens postadas no Yammer
- Contagem de mensagens lidas no Yammer
- Contagem de mensagens curtidas no Yammer
- Quantidade de itens totais da caixa de correio do Exchange
- Armazenamento utilizado da caixa de correio do Exchange (bytes)
- Contagem total de arquivos do SharePoint
- Armazenamento utilizado do site do SharePoint (bytes)
- Período de Relatório

Não há suporte para as seguintes colunas na China Microsoft Graph operado pela 21Vianet:

- Contagem de mensagens postadas no Yammer
- Contagem de mensagens lidas no Yammer
- Contagem de mensagens curtidas no Yammer

### <a name="json"></a>JSON

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** no corpo da resposta.

Não há suporte para as seguintes propriedades no objeto **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** na China Microsoft Graph operado pela 21Vianet:

- yammerPostedMessageCount
- yammerReadMessageCount
- yammerLikedMessageCount

O tamanho de página padrão para essa solicitação é 200 itens.

## <a name="example"></a>Exemplo

### <a name="csv"></a>CSV

O exemplo a seguir é um exemplo que emite CSV.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
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

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,External Member Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```

### <a name="json"></a>JSON

O exemplo a seguir é um exemplo que retorne JSON.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 674

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerDisplayName-value", 
      "lastActivityDate": "2017-08-31", 
      "groupType": "Private", 
      "memberCount": 5, 
      "externalMemberCount": 0, 
      "exchangeReceivedEmailCount": 341, 
      "sharePointActiveFileCount": 0, 
      "yammerPostedMessageCount": 0, 
      "yammerReadMessageCount": 0, 
      "yammerLikedMessageCount": 0, 
      "exchangeMailboxTotalItemCount": 343, 
      "exchangeMailboxStorageUsedInBytes": 3724609, 
      "sharePointTotalFileCount": 0, 
      "sharePointSiteStorageUsedInBytes": 0, 
      "reportPeriod": "30"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
