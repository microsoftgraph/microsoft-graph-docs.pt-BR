---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 4bbbc7cadac13134286c49aa58745c4f57a7c65c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050959"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="3f1ba-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="3f1ba-103">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="3f1ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f1ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f1ba-105">Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-105">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="3f1ba-106">**Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="3f1ba-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="3f1ba-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f1ba-107">Permissions</span></span>

<span data-ttu-id="3f1ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f1ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f1ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f1ba-110">Permission type</span></span>                        | <span data-ttu-id="3f1ba-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f1ba-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3f1ba-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f1ba-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f1ba-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f1ba-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3f1ba-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f1ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f1ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-115">Not supported.</span></span>                           |
| <span data-ttu-id="3f1ba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f1ba-116">Application</span></span>                            | <span data-ttu-id="3f1ba-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f1ba-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="3f1ba-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3f1ba-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3f1ba-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3f1ba-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f1ba-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="3f1ba-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3f1ba-121">Function parameters</span></span>

<span data-ttu-id="3f1ba-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="3f1ba-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3f1ba-123">Parameter</span></span> | <span data-ttu-id="3f1ba-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f1ba-124">Type</span></span>   | <span data-ttu-id="3f1ba-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f1ba-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3f1ba-126">ponto</span><span class="sxs-lookup"><span data-stu-id="3f1ba-126">period</span></span>    | <span data-ttu-id="3f1ba-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f1ba-127">string</span></span> | <span data-ttu-id="3f1ba-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3f1ba-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3f1ba-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="3f1ba-131">data</span><span class="sxs-lookup"><span data-stu-id="3f1ba-131">date</span></span>      | <span data-ttu-id="3f1ba-132">Data</span><span class="sxs-lookup"><span data-stu-id="3f1ba-132">Date</span></span>   | <span data-ttu-id="3f1ba-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="3f1ba-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="3f1ba-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="3f1ba-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="3f1ba-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3f1ba-138">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-138">The default output type is text/csv.</span></span> <span data-ttu-id="3f1ba-139">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f1ba-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f1ba-140">Request headers</span></span>

| <span data-ttu-id="3f1ba-141">Nome</span><span class="sxs-lookup"><span data-stu-id="3f1ba-141">Name</span></span>          | <span data-ttu-id="3f1ba-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f1ba-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3f1ba-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f1ba-143">Authorization</span></span> | <span data-ttu-id="3f1ba-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3f1ba-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f1ba-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3f1ba-147">CSV</span><span class="sxs-lookup"><span data-stu-id="3f1ba-147">CSV</span></span>

<span data-ttu-id="3f1ba-148">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3f1ba-149">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3f1ba-150">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3f1ba-151">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3f1ba-152">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3f1ba-152">Report Refresh Date</span></span>
- <span data-ttu-id="3f1ba-153">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="3f1ba-153">User Principal Name</span></span>
- <span data-ttu-id="3f1ba-154">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="3f1ba-154">Display Name</span></span>
- <span data-ttu-id="3f1ba-155">Excluído</span><span class="sxs-lookup"><span data-stu-id="3f1ba-155">Is Deleted</span></span>
- <span data-ttu-id="3f1ba-156">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="3f1ba-156">Deleted Date</span></span>
- <span data-ttu-id="3f1ba-157">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="3f1ba-157">Last Activity Date</span></span>
- <span data-ttu-id="3f1ba-158">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="3f1ba-158">Mail For Mac</span></span>
- <span data-ttu-id="3f1ba-159">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="3f1ba-159">Outlook For Mac</span></span>
- <span data-ttu-id="3f1ba-160">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="3f1ba-160">Outlook For Windows</span></span>
- <span data-ttu-id="3f1ba-161">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="3f1ba-161">Outlook For Mobile</span></span>
- <span data-ttu-id="3f1ba-162">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="3f1ba-162">Other For Mobile</span></span>
- <span data-ttu-id="3f1ba-163">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="3f1ba-163">Outlook For Web</span></span>
- <span data-ttu-id="3f1ba-164">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="3f1ba-164">POP3 App</span></span>
- <span data-ttu-id="3f1ba-165">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="3f1ba-165">IMAP4 App</span></span>
- <span data-ttu-id="3f1ba-166">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="3f1ba-166">SMTP App</span></span>
- <span data-ttu-id="3f1ba-167">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3f1ba-167">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3f1ba-168">JSON</span><span class="sxs-lookup"><span data-stu-id="3f1ba-168">JSON</span></span>

<span data-ttu-id="3f1ba-169">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-169">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="3f1ba-170">O tamanho padrão da página para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-170">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="3f1ba-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f1ba-171">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3f1ba-172">CSV</span><span class="sxs-lookup"><span data-stu-id="3f1ba-172">CSV</span></span>

<span data-ttu-id="3f1ba-173">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-173">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3f1ba-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f1ba-174">Request</span></span>

<span data-ttu-id="3f1ba-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-175">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="3f1ba-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f1ba-176">Response</span></span>

<span data-ttu-id="3f1ba-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-177">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3f1ba-178">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-178">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="3f1ba-179">JSON</span><span class="sxs-lookup"><span data-stu-id="3f1ba-179">JSON</span></span>

<span data-ttu-id="3f1ba-180">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-180">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3f1ba-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f1ba-181">Request</span></span>

<span data-ttu-id="3f1ba-182">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-182">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="3f1ba-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f1ba-183">Response</span></span>

<span data-ttu-id="3f1ba-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-184">The following is an example of the response.</span></span>

> <span data-ttu-id="3f1ba-185">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3f1ba-185">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 515

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "mailForMac": [ ], 
      "outlookForMac": [ ], 
      "outlookForWindows": [ ], 
      "outlookForMobile": [
        "Undetermined"
      ], 
      "otherForMobile": [ ], 
      "outlookForWeb": [
        "Undetermined"
      ], 
      "pop3App": [ ], 
      "imap4App": [ ], 
      "smtpApp": [ ], 
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


