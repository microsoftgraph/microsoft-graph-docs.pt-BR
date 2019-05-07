---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Obtenha a contagem de usuários por tipo de atividade e serviço.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9cf9af433e99db343e1ed5678f497b6d23aa7cd9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33604974"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="8c9c0-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="8c9c0-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="8c9c0-104">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="8c9c0-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="8c9c0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c9c0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c9c0-106">Permissions</span></span>

<span data-ttu-id="8c9c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c9c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c9c0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c9c0-109">Permission type</span></span>                        | <span data-ttu-id="8c9c0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c9c0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8c9c0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c9c0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c9c0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c9c0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8c9c0-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c9c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c9c0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-114">Not supported.</span></span>                           |
| <span data-ttu-id="8c9c0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-115">Application</span></span>                            | <span data-ttu-id="8c9c0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c9c0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8c9c0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c9c0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8c9c0-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8c9c0-118">Function parameters</span></span>

<span data-ttu-id="8c9c0-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8c9c0-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8c9c0-120">Parameter</span></span> | <span data-ttu-id="8c9c0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-121">Type</span></span>   | <span data-ttu-id="8c9c0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c9c0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8c9c0-123">ponto</span><span class="sxs-lookup"><span data-stu-id="8c9c0-123">period</span></span>    | <span data-ttu-id="8c9c0-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c9c0-124">string</span></span> | <span data-ttu-id="8c9c0-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8c9c0-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8c9c0-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8c9c0-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8c9c0-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c9c0-129">Request headers</span></span>

| <span data-ttu-id="8c9c0-130">Nome</span><span class="sxs-lookup"><span data-stu-id="8c9c0-130">Name</span></span>          | <span data-ttu-id="8c9c0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c9c0-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8c9c0-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c9c0-132">Authorization</span></span> | <span data-ttu-id="8c9c0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8c9c0-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8c9c0-135">If-None-Match</span></span> | <span data-ttu-id="8c9c0-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8c9c0-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8c9c0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c9c0-138">Response</span></span>

<span data-ttu-id="8c9c0-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8c9c0-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8c9c0-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8c9c0-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8c9c0-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="8c9c0-143">Report Refresh Date</span></span>
- <span data-ttu-id="8c9c0-144">Exchange ativo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-144">Exchange Active</span></span>
- <span data-ttu-id="8c9c0-145">Exchange inativo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-145">Exchange Inactive</span></span>
- <span data-ttu-id="8c9c0-146">OneDrive ativo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-146">OneDrive Active</span></span>
- <span data-ttu-id="8c9c0-147">OneDrive inativo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-147">OneDrive Inactive</span></span>
- <span data-ttu-id="8c9c0-148">SharePoint ativo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-148">SharePoint Active</span></span>
- <span data-ttu-id="8c9c0-149">SharePoint inativo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-149">SharePoint Inactive</span></span>
- <span data-ttu-id="8c9c0-150">Skype for Business ativo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-150">Skype For Business Active</span></span>
- <span data-ttu-id="8c9c0-151">Skype for Business inativo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-151">Skype For Business Inactive</span></span>
- <span data-ttu-id="8c9c0-152">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="8c9c0-152">Yammer Active</span></span>
- <span data-ttu-id="8c9c0-153">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="8c9c0-153">Yammer Inactive</span></span>
- <span data-ttu-id="8c9c0-154">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-154">Teams Active</span></span>
- <span data-ttu-id="8c9c0-155">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-155">Teams Inactive</span></span>
- <span data-ttu-id="8c9c0-156">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="8c9c0-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8c9c0-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c9c0-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8c9c0-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c9c0-158">Request</span></span>

<span data-ttu-id="8c9c0-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8c9c0-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c9c0-160">Response</span></span>

<span data-ttu-id="8c9c0-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-161">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8c9c0-162">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8c9c0-162">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8c9c0-163">Basic</span><span class="sxs-lookup"><span data-stu-id="8c9c0-163">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365servicesusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c9c0-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c9c0-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365servicesusercounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="8c9c0-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="8c9c0-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365servicesusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365servicesusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
