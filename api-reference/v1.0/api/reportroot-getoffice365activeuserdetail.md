---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Obter detalhes sobre usuários ativos do Microsoft 365.
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 4553207f0c31b35feb8653a25d6ec1afa2e656a4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130283"
---
# <a name="reportroot-getoffice365activeuserdetail"></a>reportRoot: getOffice365ActiveUserDetail

Namespace: microsoft.graph

Obter detalhes sobre usuários ativos do Microsoft 365.

> **Observação:** Para saber mais sobre os diferentes modos de exibição de relatório e nomes, confira [Relatórios do Microsoft 365 - Usuários Ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d). 

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
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a>Parâmetros de função

Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.

| Parâmetro | Tipo   | Descrição                              |
| :-------- | :----- | :--------------------------------------- |
| ponto    | cadeia de caracteres | Especifica o período de tempo durante o qual o relatório é agregado. Os valores com suporte para {period_value} são: D7, D30, D90 e D180. Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado. |
| data      | Data   | Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade. {date_value} deve ter um formato de AAAA-MM-DD. Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo. |

> **Observação:** você precisa definir o período ou data na URL.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                              |
| :------------ | :--------------------------------------- |
| Autorização | {token} de portador. Obrigatório.                |
| If-None-Match | Se esse cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido. Opcional. |

## <a name="response"></a>Resposta

Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório. Essa URL pode ser encontrada no cabeçalho `Location` na resposta.

As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.

O arquivo CSV possui os seguintes cabeçalhos para colunas.

- Data de atualização do relatório
- Nome UPN
- Nome de exibição
- Excluído
- Data de exclusão
- Tem a licença do Exchange
- Tem a licença do OneDrive
- Tem a licença do SharePoint
- Tem a licença do Skype for Business
- Tem a licença do Yammer
- Tem a licença do Teams
- Data da última atividade do Exchange
- Data da última atividade do OneDrive
- Data da última atividade do SharePoint
- Data da última atividade do Skype for Business
- Data da última atividade do Yammer
- Data da última atividade do Teams
- Data de atribuição da licença do Exchange
- Data de atribuição da licença do OneDrive
- Data de atribuição da licença do SharePoint
- Data de atribuição da licença do Skype for Business
- Data de atribuição da licença do Yammer
- Data de atribuição da licença do Teams
- Produtos Atribuídos

## <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
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

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
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

