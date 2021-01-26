---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Obtenha dados sobre o uso do dispositivo Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 3314ea443fecc1a9fc93236ac93b8c137d6cf2bc
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981414"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="416ca-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="416ca-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="416ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="416ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="416ca-105">Obtenha dados sobre o uso do dispositivo Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="416ca-105">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="416ca-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - Clientes do Skype for Business usados.](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)</span><span class="sxs-lookup"><span data-stu-id="416ca-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="416ca-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="416ca-107">Permissions</span></span>

<span data-ttu-id="416ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="416ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="416ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="416ca-110">Permission type</span></span>                        | <span data-ttu-id="416ca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="416ca-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="416ca-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="416ca-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="416ca-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="416ca-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="416ca-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="416ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="416ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="416ca-115">Not supported.</span></span>                           |
| <span data-ttu-id="416ca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="416ca-116">Application</span></span>                            | <span data-ttu-id="416ca-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="416ca-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="416ca-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="416ca-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="416ca-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="416ca-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="416ca-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="416ca-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="416ca-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="416ca-121">Function parameters</span></span>

<span data-ttu-id="416ca-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="416ca-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="416ca-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="416ca-123">Parameter</span></span> | <span data-ttu-id="416ca-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="416ca-124">Type</span></span>   | <span data-ttu-id="416ca-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="416ca-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="416ca-126">ponto</span><span class="sxs-lookup"><span data-stu-id="416ca-126">period</span></span>    | <span data-ttu-id="416ca-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="416ca-127">string</span></span> | <span data-ttu-id="416ca-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="416ca-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="416ca-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="416ca-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="416ca-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="416ca-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="416ca-131">data</span><span class="sxs-lookup"><span data-stu-id="416ca-131">date</span></span>      | <span data-ttu-id="416ca-132">Data</span><span class="sxs-lookup"><span data-stu-id="416ca-132">Date</span></span>   | <span data-ttu-id="416ca-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="416ca-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="416ca-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="416ca-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="416ca-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="416ca-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="416ca-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="416ca-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="416ca-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="416ca-137">Request headers</span></span>

| <span data-ttu-id="416ca-138">Nome</span><span class="sxs-lookup"><span data-stu-id="416ca-138">Name</span></span>          | <span data-ttu-id="416ca-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="416ca-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="416ca-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="416ca-140">Authorization</span></span> | <span data-ttu-id="416ca-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="416ca-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="416ca-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="416ca-143">If-None-Match</span></span> | <span data-ttu-id="416ca-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="416ca-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="416ca-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="416ca-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="416ca-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="416ca-146">Response</span></span>

<span data-ttu-id="416ca-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="416ca-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="416ca-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="416ca-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="416ca-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="416ca-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="416ca-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="416ca-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="416ca-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="416ca-151">Report Refresh Date</span></span>
- <span data-ttu-id="416ca-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="416ca-152">User Principal Name</span></span>
- <span data-ttu-id="416ca-153">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="416ca-153">Last Activity Date</span></span>
- <span data-ttu-id="416ca-154">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="416ca-154">Used Windows</span></span>
- <span data-ttu-id="416ca-155">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="416ca-155">Used Windows Phone</span></span>
- <span data-ttu-id="416ca-156">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="416ca-156">Used Android Phone</span></span>
- <span data-ttu-id="416ca-157">Usou iPhone</span><span class="sxs-lookup"><span data-stu-id="416ca-157">Used iPhone</span></span>
- <span data-ttu-id="416ca-158">Usou iPad</span><span class="sxs-lookup"><span data-stu-id="416ca-158">Used iPad</span></span>
- <span data-ttu-id="416ca-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="416ca-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="416ca-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="416ca-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="416ca-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="416ca-161">Request</span></span>

<span data-ttu-id="416ca-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="416ca-162">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="416ca-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="416ca-163">Response</span></span>

<span data-ttu-id="416ca-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="416ca-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="416ca-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="416ca-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
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

