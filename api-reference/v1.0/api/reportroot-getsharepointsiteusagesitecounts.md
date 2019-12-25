---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e09cc1881b786b7cfdfff6057d1aff8663b8a1e4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865325"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="e9ac5-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="e9ac5-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="e9ac5-105">Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="e9ac5-106">Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="e9ac5-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="e9ac5-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9ac5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9ac5-108">Permissions</span></span>

<span data-ttu-id="e9ac5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9ac5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9ac5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9ac5-111">Permission type</span></span>                        | <span data-ttu-id="e9ac5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9ac5-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e9ac5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9ac5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9ac5-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9ac5-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e9ac5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9ac5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9ac5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-116">Not supported.</span></span>                           |
| <span data-ttu-id="e9ac5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9ac5-117">Application</span></span>                            | <span data-ttu-id="e9ac5-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9ac5-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="e9ac5-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e9ac5-120">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="e9ac5-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e9ac5-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9ac5-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e9ac5-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e9ac5-122">Function parameters</span></span>

<span data-ttu-id="e9ac5-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e9ac5-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e9ac5-124">Parameter</span></span> | <span data-ttu-id="e9ac5-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9ac5-125">Type</span></span>   | <span data-ttu-id="e9ac5-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9ac5-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e9ac5-127">ponto</span><span class="sxs-lookup"><span data-stu-id="e9ac5-127">period</span></span>    | <span data-ttu-id="e9ac5-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9ac5-128">string</span></span> | <span data-ttu-id="e9ac5-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e9ac5-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e9ac5-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e9ac5-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e9ac5-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9ac5-133">Request headers</span></span>

| <span data-ttu-id="e9ac5-134">Nome</span><span class="sxs-lookup"><span data-stu-id="e9ac5-134">Name</span></span>          | <span data-ttu-id="e9ac5-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9ac5-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e9ac5-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9ac5-136">Authorization</span></span> | <span data-ttu-id="e9ac5-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e9ac5-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e9ac5-139">If-None-Match</span></span> | <span data-ttu-id="e9ac5-140">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e9ac5-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e9ac5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9ac5-142">Response</span></span>

<span data-ttu-id="e9ac5-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e9ac5-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e9ac5-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e9ac5-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e9ac5-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e9ac5-147">Report Refresh Date</span></span>
- <span data-ttu-id="e9ac5-148">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="e9ac5-148">Site Type</span></span>
- <span data-ttu-id="e9ac5-149">Total</span><span class="sxs-lookup"><span data-stu-id="e9ac5-149">Total</span></span>
- <span data-ttu-id="e9ac5-150">Ativo</span><span class="sxs-lookup"><span data-stu-id="e9ac5-150">Active</span></span>
- <span data-ttu-id="e9ac5-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="e9ac5-151">Report Date</span></span>
- <span data-ttu-id="e9ac5-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e9ac5-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e9ac5-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9ac5-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e9ac5-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9ac5-154">Request</span></span>

<span data-ttu-id="e9ac5-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e9ac5-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9ac5-156">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e9ac5-157">C#</span><span class="sxs-lookup"><span data-stu-id="e9ac5-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagesitecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9ac5-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9ac5-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagesitecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e9ac5-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9ac5-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagesitecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e9ac5-160">Java</span><span class="sxs-lookup"><span data-stu-id="e9ac5-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagesitecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9ac5-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9ac5-161">Response</span></span>

<span data-ttu-id="e9ac5-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-162">The following is an example of the response.</span></span>

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

<span data-ttu-id="e9ac5-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e9ac5-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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
