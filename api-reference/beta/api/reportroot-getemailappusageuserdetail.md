---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 73ba77656b15f8c5de6db0aac50f94afc8a9228a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331677"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="16fa0-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="16fa0-103">reportRoot: getEmailAppUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16fa0-104">Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.</span><span class="sxs-lookup"><span data-stu-id="16fa0-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="16fa0-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="16fa0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="16fa0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="16fa0-106">Permissions</span></span>

<span data-ttu-id="16fa0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16fa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16fa0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16fa0-109">Permission type</span></span>                        | <span data-ttu-id="16fa0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16fa0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="16fa0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16fa0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="16fa0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="16fa0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="16fa0-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16fa0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16fa0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16fa0-114">Not supported.</span></span>                           |
| <span data-ttu-id="16fa0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16fa0-115">Application</span></span>                            | <span data-ttu-id="16fa0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="16fa0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="16fa0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16fa0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="16fa0-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="16fa0-118">Function parameters</span></span>

<span data-ttu-id="16fa0-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="16fa0-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="16fa0-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="16fa0-120">Parameter</span></span> | <span data-ttu-id="16fa0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="16fa0-121">Type</span></span>   | <span data-ttu-id="16fa0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="16fa0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="16fa0-123">ponto</span><span class="sxs-lookup"><span data-stu-id="16fa0-123">period</span></span>    | <span data-ttu-id="16fa0-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16fa0-124">string</span></span> | <span data-ttu-id="16fa0-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="16fa0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="16fa0-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="16fa0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="16fa0-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="16fa0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="16fa0-128">data</span><span class="sxs-lookup"><span data-stu-id="16fa0-128">date</span></span>      | <span data-ttu-id="16fa0-129">Data</span><span class="sxs-lookup"><span data-stu-id="16fa0-129">Date</span></span>   | <span data-ttu-id="16fa0-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="16fa0-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="16fa0-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="16fa0-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="16fa0-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="16fa0-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="16fa0-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="16fa0-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="16fa0-134">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="16fa0-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="16fa0-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="16fa0-135">The default output type is text/csv.</span></span> <span data-ttu-id="16fa0-136">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="16fa0-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16fa0-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16fa0-137">Request headers</span></span>

| <span data-ttu-id="16fa0-138">Nome</span><span class="sxs-lookup"><span data-stu-id="16fa0-138">Name</span></span>          | <span data-ttu-id="16fa0-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="16fa0-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="16fa0-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="16fa0-140">Authorization</span></span> | <span data-ttu-id="16fa0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16fa0-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="16fa0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="16fa0-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="16fa0-144">CSV</span><span class="sxs-lookup"><span data-stu-id="16fa0-144">CSV</span></span>

<span data-ttu-id="16fa0-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="16fa0-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="16fa0-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="16fa0-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="16fa0-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="16fa0-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="16fa0-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="16fa0-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="16fa0-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="16fa0-149">Report Refresh Date</span></span>
- <span data-ttu-id="16fa0-150">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="16fa0-150">User Principal Name</span></span>
- <span data-ttu-id="16fa0-151">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="16fa0-151">Display Name</span></span>
- <span data-ttu-id="16fa0-152">Excluído</span><span class="sxs-lookup"><span data-stu-id="16fa0-152">Is Deleted</span></span>
- <span data-ttu-id="16fa0-153">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="16fa0-153">Deleted Date</span></span>
- <span data-ttu-id="16fa0-154">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="16fa0-154">Last Activity Date</span></span>
- <span data-ttu-id="16fa0-155">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="16fa0-155">Mail For Mac</span></span>
- <span data-ttu-id="16fa0-156">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="16fa0-156">Outlook For Mac</span></span>
- <span data-ttu-id="16fa0-157">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="16fa0-157">Outlook For Windows</span></span>
- <span data-ttu-id="16fa0-158">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="16fa0-158">Outlook For Mobile</span></span>
- <span data-ttu-id="16fa0-159">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="16fa0-159">Other For Mobile</span></span>
- <span data-ttu-id="16fa0-160">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="16fa0-160">Outlook For Web</span></span>
- <span data-ttu-id="16fa0-161">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="16fa0-161">POP3 App</span></span>
- <span data-ttu-id="16fa0-162">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="16fa0-162">IMAP4 App</span></span>
- <span data-ttu-id="16fa0-163">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="16fa0-163">SMTP App</span></span>
- <span data-ttu-id="16fa0-164">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="16fa0-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="16fa0-165">JSON</span><span class="sxs-lookup"><span data-stu-id="16fa0-165">JSON</span></span>

<span data-ttu-id="16fa0-166">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16fa0-166">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="16fa0-167">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="16fa0-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="16fa0-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16fa0-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="16fa0-169">CSV</span><span class="sxs-lookup"><span data-stu-id="16fa0-169">CSV</span></span>

<span data-ttu-id="16fa0-170">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="16fa0-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="16fa0-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16fa0-171">Request</span></span>

<span data-ttu-id="16fa0-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="16fa0-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="16fa0-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="16fa0-173">Response</span></span>

<span data-ttu-id="16fa0-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="16fa0-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="16fa0-175">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="16fa0-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="16fa0-176">JSON</span><span class="sxs-lookup"><span data-stu-id="16fa0-176">JSON</span></span>

<span data-ttu-id="16fa0-177">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="16fa0-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="16fa0-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16fa0-178">Request</span></span>

<span data-ttu-id="16fa0-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="16fa0-179">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="16fa0-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="16fa0-180">Response</span></span>

<span data-ttu-id="16fa0-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="16fa0-181">The following is an example of the response.</span></span>

> <span data-ttu-id="16fa0-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16fa0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
