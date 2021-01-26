---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 6f40ddf0a8ae93f39b56f57e2f97b4d1b6e08052
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981799"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="7eb7d-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="7eb7d-103">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="7eb7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eb7d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7eb7d-105">Obtenha dados sobre quais atividades os usuários realizaram nos vários aplicativos de email.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-105">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="7eb7d-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - Uso de aplicativos de email.](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)</span><span class="sxs-lookup"><span data-stu-id="7eb7d-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="7eb7d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7eb7d-107">Permissions</span></span>

<span data-ttu-id="7eb7d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7eb7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7eb7d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7eb7d-110">Permission type</span></span>                        | <span data-ttu-id="7eb7d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7eb7d-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7eb7d-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7eb7d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7eb7d-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7eb7d-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7eb7d-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7eb7d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7eb7d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-115">Not supported.</span></span>                           |
| <span data-ttu-id="7eb7d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7eb7d-116">Application</span></span>                            | <span data-ttu-id="7eb7d-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7eb7d-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="7eb7d-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7eb7d-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="7eb7d-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7eb7d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7eb7d-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7eb7d-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7eb7d-121">Function parameters</span></span>

<span data-ttu-id="7eb7d-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7eb7d-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7eb7d-123">Parameter</span></span> | <span data-ttu-id="7eb7d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="7eb7d-124">Type</span></span>   | <span data-ttu-id="7eb7d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eb7d-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7eb7d-126">ponto</span><span class="sxs-lookup"><span data-stu-id="7eb7d-126">period</span></span>    | <span data-ttu-id="7eb7d-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7eb7d-127">string</span></span> | <span data-ttu-id="7eb7d-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7eb7d-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7eb7d-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7eb7d-131">data</span><span class="sxs-lookup"><span data-stu-id="7eb7d-131">date</span></span>      | <span data-ttu-id="7eb7d-132">Data</span><span class="sxs-lookup"><span data-stu-id="7eb7d-132">Date</span></span>   | <span data-ttu-id="7eb7d-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7eb7d-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7eb7d-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7eb7d-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7eb7d-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7eb7d-137">Request headers</span></span>

| <span data-ttu-id="7eb7d-138">Nome</span><span class="sxs-lookup"><span data-stu-id="7eb7d-138">Name</span></span>          | <span data-ttu-id="7eb7d-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eb7d-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7eb7d-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="7eb7d-140">Authorization</span></span> | <span data-ttu-id="7eb7d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7eb7d-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7eb7d-143">If-None-Match</span></span> | <span data-ttu-id="7eb7d-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7eb7d-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7eb7d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7eb7d-146">Response</span></span>

<span data-ttu-id="7eb7d-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7eb7d-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7eb7d-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7eb7d-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7eb7d-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7eb7d-151">Report Refresh Date</span></span>
- <span data-ttu-id="7eb7d-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="7eb7d-152">User Principal Name</span></span>
- <span data-ttu-id="7eb7d-153">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="7eb7d-153">Display Name</span></span>
- <span data-ttu-id="7eb7d-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="7eb7d-154">Is Deleted</span></span>
- <span data-ttu-id="7eb7d-155">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="7eb7d-155">Deleted Date</span></span>
- <span data-ttu-id="7eb7d-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="7eb7d-156">Last Activity Date</span></span>
- <span data-ttu-id="7eb7d-157">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="7eb7d-157">Mail For Mac</span></span>
- <span data-ttu-id="7eb7d-158">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="7eb7d-158">Outlook For Mac</span></span>
- <span data-ttu-id="7eb7d-159">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="7eb7d-159">Outlook For Windows</span></span>
- <span data-ttu-id="7eb7d-160">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="7eb7d-160">Outlook For Mobile</span></span>
- <span data-ttu-id="7eb7d-161">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="7eb7d-161">Other For Mobile</span></span>
- <span data-ttu-id="7eb7d-162">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="7eb7d-162">Outlook For Web</span></span>
- <span data-ttu-id="7eb7d-163">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="7eb7d-163">POP3 App</span></span>
- <span data-ttu-id="7eb7d-164">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="7eb7d-164">IMAP4 App</span></span>
- <span data-ttu-id="7eb7d-165">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="7eb7d-165">SMTP App</span></span>
- <span data-ttu-id="7eb7d-166">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7eb7d-166">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7eb7d-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7eb7d-167">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7eb7d-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7eb7d-168">Request</span></span>

<span data-ttu-id="7eb7d-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-169">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getemailappusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="7eb7d-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="7eb7d-170">Response</span></span>

<span data-ttu-id="7eb7d-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-171">The following is an example of the response.</span></span>

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

<span data-ttu-id="7eb7d-172">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7eb7d-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
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

