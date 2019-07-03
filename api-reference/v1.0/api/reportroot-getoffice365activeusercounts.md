---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Obtenha a contagem de usuários ativos diários no período de relatório por produto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a031018a55e29b9237fa6c4a9ebca51c069d7917
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459213"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="79058-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="79058-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="79058-104">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="79058-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="79058-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="79058-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="79058-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="79058-106">Permissions</span></span>

<span data-ttu-id="79058-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79058-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79058-109">Permission type</span></span>                        | <span data-ttu-id="79058-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79058-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="79058-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79058-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="79058-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="79058-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="79058-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79058-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79058-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79058-114">Not supported.</span></span>                           |
| <span data-ttu-id="79058-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79058-115">Application</span></span>                            | <span data-ttu-id="79058-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="79058-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="79058-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79058-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="79058-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="79058-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="79058-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="79058-119">Function parameters</span></span>

<span data-ttu-id="79058-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="79058-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="79058-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="79058-121">Parameter</span></span> | <span data-ttu-id="79058-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="79058-122">Type</span></span>   | <span data-ttu-id="79058-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="79058-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="79058-124">ponto</span><span class="sxs-lookup"><span data-stu-id="79058-124">period</span></span>    | <span data-ttu-id="79058-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79058-125">string</span></span> | <span data-ttu-id="79058-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="79058-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="79058-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="79058-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="79058-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="79058-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="79058-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79058-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="79058-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79058-130">Request headers</span></span>

| <span data-ttu-id="79058-131">Nome</span><span class="sxs-lookup"><span data-stu-id="79058-131">Name</span></span>          | <span data-ttu-id="79058-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="79058-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="79058-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="79058-133">Authorization</span></span> | <span data-ttu-id="79058-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79058-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="79058-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="79058-136">Response</span></span>

<span data-ttu-id="79058-137">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="79058-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="79058-138">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="79058-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="79058-139">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="79058-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="79058-140">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="79058-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="79058-141">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="79058-141">Report Refresh Date</span></span>
- <span data-ttu-id="79058-142">Office 365</span><span class="sxs-lookup"><span data-stu-id="79058-142">Office 365</span></span>
- <span data-ttu-id="79058-143">Exchange</span><span class="sxs-lookup"><span data-stu-id="79058-143">Exchange</span></span>
- <span data-ttu-id="79058-144">OneDrive</span><span class="sxs-lookup"><span data-stu-id="79058-144">OneDrive</span></span>
- <span data-ttu-id="79058-145">SharePoint</span><span class="sxs-lookup"><span data-stu-id="79058-145">SharePoint</span></span>
- <span data-ttu-id="79058-146">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="79058-146">Skype For Business</span></span> 
- <span data-ttu-id="79058-147">Yammer</span><span class="sxs-lookup"><span data-stu-id="79058-147">Yammer</span></span>
- <span data-ttu-id="79058-148">Teams</span><span class="sxs-lookup"><span data-stu-id="79058-148">Teams</span></span>
- <span data-ttu-id="79058-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="79058-149">Report Date</span></span>
- <span data-ttu-id="79058-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="79058-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="79058-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79058-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="79058-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79058-152">Request</span></span>

<span data-ttu-id="79058-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79058-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79058-154">C#</span><span class="sxs-lookup"><span data-stu-id="79058-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79058-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="79058-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79058-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="79058-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79058-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="79058-157">Response</span></span>

<span data-ttu-id="79058-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="79058-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="79058-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="79058-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
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
