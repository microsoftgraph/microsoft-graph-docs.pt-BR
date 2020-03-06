---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 482a7dcb319f243222b656be1880ed6e83eaa96c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510197"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="c7304-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="c7304-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="c7304-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7304-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7304-106">Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos.</span><span class="sxs-lookup"><span data-stu-id="c7304-106">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="c7304-107">Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="c7304-107">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="c7304-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="c7304-108">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7304-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7304-109">Permissions</span></span>

<span data-ttu-id="c7304-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7304-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7304-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7304-112">Permission type</span></span>                        | <span data-ttu-id="c7304-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7304-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c7304-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7304-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7304-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7304-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c7304-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7304-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7304-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7304-117">Not supported.</span></span>                           |
| <span data-ttu-id="c7304-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7304-118">Application</span></span>                            | <span data-ttu-id="c7304-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7304-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="c7304-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="c7304-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="c7304-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="c7304-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="c7304-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7304-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c7304-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c7304-123">Function parameters</span></span>

<span data-ttu-id="c7304-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="c7304-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c7304-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c7304-125">Parameter</span></span> | <span data-ttu-id="c7304-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7304-126">Type</span></span>   | <span data-ttu-id="c7304-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7304-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c7304-128">ponto</span><span class="sxs-lookup"><span data-stu-id="c7304-128">period</span></span>    | <span data-ttu-id="c7304-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7304-129">string</span></span> | <span data-ttu-id="c7304-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c7304-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c7304-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="c7304-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c7304-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c7304-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c7304-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7304-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c7304-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7304-134">Request headers</span></span>

| <span data-ttu-id="c7304-135">Nome</span><span class="sxs-lookup"><span data-stu-id="c7304-135">Name</span></span>          | <span data-ttu-id="c7304-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7304-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c7304-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7304-137">Authorization</span></span> | <span data-ttu-id="c7304-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7304-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c7304-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c7304-140">If-None-Match</span></span> | <span data-ttu-id="c7304-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="c7304-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c7304-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c7304-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c7304-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7304-143">Response</span></span>

<span data-ttu-id="c7304-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="c7304-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c7304-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c7304-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c7304-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c7304-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c7304-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="c7304-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c7304-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="c7304-148">Report Refresh Date</span></span>
- <span data-ttu-id="c7304-149">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="c7304-149">Site Type</span></span>
- <span data-ttu-id="c7304-150">Total</span><span class="sxs-lookup"><span data-stu-id="c7304-150">Total</span></span>
- <span data-ttu-id="c7304-151">Ativo</span><span class="sxs-lookup"><span data-stu-id="c7304-151">Active</span></span>
- <span data-ttu-id="c7304-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="c7304-152">Report Date</span></span>
- <span data-ttu-id="c7304-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="c7304-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c7304-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7304-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c7304-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7304-155">Request</span></span>

<span data-ttu-id="c7304-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7304-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c7304-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7304-157">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="c7304-158">C#</span><span class="sxs-lookup"><span data-stu-id="c7304-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagesitecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7304-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7304-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagesitecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7304-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7304-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagesitecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7304-161">Java</span><span class="sxs-lookup"><span data-stu-id="c7304-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagesitecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c7304-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7304-162">Response</span></span>

<span data-ttu-id="c7304-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7304-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="c7304-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="c7304-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
