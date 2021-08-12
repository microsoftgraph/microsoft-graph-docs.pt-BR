---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Obter detalhes sobre a atividade de usuário do Microsoft Teams por usuário.
localization_priority: Priority
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: f7f55c67e6e9b13c21fcd58b65806c2b0379ac7465da35de197be9f5e2778049
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240621"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a>reportRoot: getTeamsUserActivityUserDetail

Namespace: microsoft.graph

Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :--------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All                         |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                           |
| Aplicativo                            | Reports.Read.All                         |

**Observação**: para as permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador de locatários deve ter atribuído ao usuário a função de administrador limitada apropriada do Azure AD. Para obter mais detalhes, consulte [Autorização para as APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a>Parâmetros de função

Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.

| Parâmetro | Tipo   | Descrição                              |
| :-------- | :----- | :--------------------------------------- |
| ponto    | cadeia de caracteres | Especifica o período de tempo durante o qual o relatório é agregado. Os valores com suporte para {period_value} são: D7, D30, D90 e D180. Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado. |
| data      | Data   | Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade. {date_value} deve ter um formato de AAAA-MM-DD. Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo. |

> **Observação:** você precisa definir o período ou data na URL.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="response"></a>Resposta

Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório. Essa URL pode ser encontrada no cabeçalho `Location` na resposta.

As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.

O arquivo CSV possui os seguintes cabeçalhos para colunas:

- Data de atualização do relatório
- Nome UPN
- Data da última atividade
- Excluído
- Data de exclusão
- Produtos Atribuídos
- Número de mensagens de chat de equipe
- Contagem de mensagens de chat privadas
- Contagem de chamadas
- Contagem de reuniões
- Tem outra ação
- Período de Relatório

## <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
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

