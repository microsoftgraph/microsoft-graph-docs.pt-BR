---
title: 'reportRoot: getOffice365GroupsActivityGroupCounts'
description: Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 27d3f6ac4dcdbc0fca92eb87deccef17626c050f
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729676"
---
# <a name="reportroot-getoffice365groupsactivitygroupcounts"></a><span data-ttu-id="0c7ee-103">reportRoot: getOffice365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="0c7ee-103">reportRoot: getOffice365GroupsActivityGroupCounts</span></span>

<span data-ttu-id="0c7ee-104">Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-104">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span>

> <span data-ttu-id="0c7ee-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="0c7ee-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="0c7ee-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c7ee-106">Permissions</span></span>

<span data-ttu-id="0c7ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c7ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c7ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c7ee-109">Permission type</span></span>                        | <span data-ttu-id="0c7ee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c7ee-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0c7ee-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c7ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c7ee-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7ee-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0c7ee-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c7ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c7ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-114">Not supported.</span></span>                           |
| <span data-ttu-id="0c7ee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c7ee-115">Application</span></span>                            | <span data-ttu-id="0c7ee-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c7ee-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0c7ee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c7ee-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0c7ee-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0c7ee-118">Function parameters</span></span>

<span data-ttu-id="0c7ee-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0c7ee-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0c7ee-120">Parameter</span></span> | <span data-ttu-id="0c7ee-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c7ee-121">Type</span></span>   | <span data-ttu-id="0c7ee-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c7ee-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0c7ee-123">ponto</span><span class="sxs-lookup"><span data-stu-id="0c7ee-123">period</span></span>    | <span data-ttu-id="0c7ee-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c7ee-124">string</span></span> | <span data-ttu-id="0c7ee-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0c7ee-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0c7ee-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0c7ee-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0c7ee-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c7ee-129">Request headers</span></span>

| <span data-ttu-id="0c7ee-130">Nome</span><span class="sxs-lookup"><span data-stu-id="0c7ee-130">Name</span></span>          | <span data-ttu-id="0c7ee-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c7ee-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0c7ee-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c7ee-132">Authorization</span></span> | <span data-ttu-id="0c7ee-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0c7ee-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0c7ee-135">If-None-Match</span></span> | <span data-ttu-id="0c7ee-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0c7ee-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0c7ee-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c7ee-138">Response</span></span>

<span data-ttu-id="0c7ee-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0c7ee-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0c7ee-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0c7ee-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0c7ee-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="0c7ee-143">Report Refresh Date</span></span>
- <span data-ttu-id="0c7ee-144">Total</span><span class="sxs-lookup"><span data-stu-id="0c7ee-144">Total</span></span>
- <span data-ttu-id="0c7ee-145">Ativo</span><span class="sxs-lookup"><span data-stu-id="0c7ee-145">Active</span></span>
- <span data-ttu-id="0c7ee-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="0c7ee-146">Report Date</span></span>
- <span data-ttu-id="0c7ee-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="0c7ee-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0c7ee-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c7ee-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0c7ee-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c7ee-149">Request</span></span>

<span data-ttu-id="0c7ee-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-150">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0c7ee-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c7ee-151">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitygroupcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityGroupCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c7ee-152">C#</span><span class="sxs-lookup"><span data-stu-id="0c7ee-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitygroupcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c7ee-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c7ee-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitygroupcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c7ee-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0c7ee-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitygroupcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0c7ee-155">Java</span><span class="sxs-lookup"><span data-stu-id="0c7ee-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivitygroupcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0c7ee-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c7ee-156">Response</span></span>

<span data-ttu-id="0c7ee-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="0c7ee-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="0c7ee-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
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
