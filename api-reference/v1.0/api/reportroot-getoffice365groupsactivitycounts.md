---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ea2bb93c93c6532a241e5141a4e45436183b93be
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893967"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="3c214-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="3c214-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

<span data-ttu-id="3c214-104">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="3c214-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="3c214-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="3c214-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c214-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c214-106">Permissions</span></span>

<span data-ttu-id="3c214-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c214-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c214-109">Permission type</span></span>                        | <span data-ttu-id="3c214-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c214-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3c214-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c214-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c214-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c214-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3c214-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c214-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c214-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c214-114">Not supported.</span></span>                           |
| <span data-ttu-id="3c214-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c214-115">Application</span></span>                            | <span data-ttu-id="3c214-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c214-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3c214-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c214-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3c214-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c214-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3c214-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3c214-119">Function parameters</span></span>

<span data-ttu-id="3c214-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3c214-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3c214-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3c214-121">Parameter</span></span> | <span data-ttu-id="3c214-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c214-122">Type</span></span>   | <span data-ttu-id="3c214-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c214-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3c214-124">ponto</span><span class="sxs-lookup"><span data-stu-id="3c214-124">period</span></span>    | <span data-ttu-id="3c214-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c214-125">string</span></span> | <span data-ttu-id="3c214-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3c214-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3c214-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3c214-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3c214-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3c214-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3c214-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c214-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3c214-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c214-130">Request headers</span></span>

| <span data-ttu-id="3c214-131">Nome</span><span class="sxs-lookup"><span data-stu-id="3c214-131">Name</span></span>          | <span data-ttu-id="3c214-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c214-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3c214-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c214-133">Authorization</span></span> | <span data-ttu-id="3c214-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c214-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3c214-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3c214-136">If-None-Match</span></span> | <span data-ttu-id="3c214-137">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="3c214-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3c214-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3c214-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3c214-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c214-139">Response</span></span>

<span data-ttu-id="3c214-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3c214-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3c214-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3c214-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3c214-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3c214-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3c214-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3c214-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3c214-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3c214-144">Report Refresh Date</span></span>
- <span data-ttu-id="3c214-145">Emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="3c214-145">Exchange Emails Received</span></span>
- <span data-ttu-id="3c214-146">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="3c214-146">Yammer Messages Posted</span></span>
- <span data-ttu-id="3c214-147">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="3c214-147">Yammer Messages Read</span></span>
- <span data-ttu-id="3c214-148">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="3c214-148">Yammer Messages Liked</span></span>
- <span data-ttu-id="3c214-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="3c214-149">Report Date</span></span>
- <span data-ttu-id="3c214-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3c214-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3c214-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c214-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3c214-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c214-152">Request</span></span>

<span data-ttu-id="3c214-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c214-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c214-154">C#</span><span class="sxs-lookup"><span data-stu-id="3c214-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitycounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c214-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c214-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitycounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c214-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3c214-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitycounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3c214-157">Java</span><span class="sxs-lookup"><span data-stu-id="3c214-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivitycounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c214-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c214-158">Response</span></span>

<span data-ttu-id="3c214-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c214-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="3c214-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3c214-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
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
