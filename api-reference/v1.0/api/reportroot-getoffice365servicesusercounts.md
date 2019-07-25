---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Obtenha a contagem de usuários por tipo de atividade e serviço.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7004b47c77b5290236004afa5bdefe0d04286d87
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893787"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="b73e4-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="b73e4-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="b73e4-104">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="b73e4-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="b73e4-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="b73e4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="b73e4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b73e4-106">Permissions</span></span>

<span data-ttu-id="b73e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b73e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b73e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b73e4-109">Permission type</span></span>                        | <span data-ttu-id="b73e4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b73e4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b73e4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b73e4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b73e4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b73e4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b73e4-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b73e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b73e4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b73e4-114">Not supported.</span></span>                           |
| <span data-ttu-id="b73e4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b73e4-115">Application</span></span>                            | <span data-ttu-id="b73e4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b73e4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b73e4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b73e4-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b73e4-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="b73e4-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b73e4-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b73e4-119">Function parameters</span></span>

<span data-ttu-id="b73e4-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b73e4-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b73e4-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b73e4-121">Parameter</span></span> | <span data-ttu-id="b73e4-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b73e4-122">Type</span></span>   | <span data-ttu-id="b73e4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b73e4-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b73e4-124">ponto</span><span class="sxs-lookup"><span data-stu-id="b73e4-124">period</span></span>    | <span data-ttu-id="b73e4-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b73e4-125">string</span></span> | <span data-ttu-id="b73e4-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b73e4-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b73e4-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b73e4-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b73e4-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b73e4-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b73e4-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b73e4-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b73e4-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b73e4-130">Request headers</span></span>

| <span data-ttu-id="b73e4-131">Nome</span><span class="sxs-lookup"><span data-stu-id="b73e4-131">Name</span></span>          | <span data-ttu-id="b73e4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b73e4-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b73e4-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="b73e4-133">Authorization</span></span> | <span data-ttu-id="b73e4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b73e4-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b73e4-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b73e4-136">If-None-Match</span></span> | <span data-ttu-id="b73e4-137">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="b73e4-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b73e4-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b73e4-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b73e4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b73e4-139">Response</span></span>

<span data-ttu-id="b73e4-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b73e4-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b73e4-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b73e4-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b73e4-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b73e4-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b73e4-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b73e4-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b73e4-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b73e4-144">Report Refresh Date</span></span>
- <span data-ttu-id="b73e4-145">Exchange ativo</span><span class="sxs-lookup"><span data-stu-id="b73e4-145">Exchange Active</span></span>
- <span data-ttu-id="b73e4-146">Exchange inativo</span><span class="sxs-lookup"><span data-stu-id="b73e4-146">Exchange Inactive</span></span>
- <span data-ttu-id="b73e4-147">OneDrive ativo</span><span class="sxs-lookup"><span data-stu-id="b73e4-147">OneDrive Active</span></span>
- <span data-ttu-id="b73e4-148">OneDrive inativo</span><span class="sxs-lookup"><span data-stu-id="b73e4-148">OneDrive Inactive</span></span>
- <span data-ttu-id="b73e4-149">SharePoint ativo</span><span class="sxs-lookup"><span data-stu-id="b73e4-149">SharePoint Active</span></span>
- <span data-ttu-id="b73e4-150">SharePoint inativo</span><span class="sxs-lookup"><span data-stu-id="b73e4-150">SharePoint Inactive</span></span>
- <span data-ttu-id="b73e4-151">Skype for Business ativo</span><span class="sxs-lookup"><span data-stu-id="b73e4-151">Skype For Business Active</span></span>
- <span data-ttu-id="b73e4-152">Skype for Business inativo</span><span class="sxs-lookup"><span data-stu-id="b73e4-152">Skype For Business Inactive</span></span>
- <span data-ttu-id="b73e4-153">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="b73e4-153">Yammer Active</span></span>
- <span data-ttu-id="b73e4-154">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="b73e4-154">Yammer Inactive</span></span>
- <span data-ttu-id="b73e4-155">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="b73e4-155">Teams Active</span></span>
- <span data-ttu-id="b73e4-156">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="b73e4-156">Teams Inactive</span></span>
- <span data-ttu-id="b73e4-157">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b73e4-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b73e4-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b73e4-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b73e4-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b73e4-159">Request</span></span>

<span data-ttu-id="b73e4-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b73e4-160">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b73e4-161">C#</span><span class="sxs-lookup"><span data-stu-id="b73e4-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b73e4-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="b73e4-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b73e4-163">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b73e4-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b73e4-164">Java</span><span class="sxs-lookup"><span data-stu-id="b73e4-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365servicesusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b73e4-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="b73e4-165">Response</span></span>

<span data-ttu-id="b73e4-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b73e4-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="b73e4-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b73e4-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
