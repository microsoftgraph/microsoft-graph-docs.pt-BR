---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos. Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 5cf276791778da81a1df1f34db09bc9d5620da60
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898321"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="15ab9-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="15ab9-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="15ab9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15ab9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15ab9-106">Obtenha o número total de arquivos em todos os sites e o número de arquivos ativos.</span><span class="sxs-lookup"><span data-stu-id="15ab9-106">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="15ab9-107">Um arquivo (usuário ou sistema) é considerado ativo se ele foi salvo, sincronizado, modificado ou compartilhado dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="15ab9-107">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="15ab9-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição de relatórios e nomes, consulte [Microsoft 365 Reports-uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="15ab9-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="15ab9-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="15ab9-109">Permissions</span></span>

<span data-ttu-id="15ab9-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="15ab9-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="15ab9-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15ab9-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15ab9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15ab9-112">Permission type</span></span>                        | <span data-ttu-id="15ab9-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15ab9-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="15ab9-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15ab9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="15ab9-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="15ab9-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="15ab9-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15ab9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15ab9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15ab9-117">Not supported.</span></span>                           |
| <span data-ttu-id="15ab9-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15ab9-118">Application</span></span>                            | <span data-ttu-id="15ab9-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="15ab9-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="15ab9-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="15ab9-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="15ab9-121">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="15ab9-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="15ab9-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15ab9-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="15ab9-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="15ab9-123">Function parameters</span></span>

<span data-ttu-id="15ab9-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="15ab9-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="15ab9-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="15ab9-125">Parameter</span></span> | <span data-ttu-id="15ab9-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="15ab9-126">Type</span></span>   | <span data-ttu-id="15ab9-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ab9-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="15ab9-128">ponto</span><span class="sxs-lookup"><span data-stu-id="15ab9-128">period</span></span>    | <span data-ttu-id="15ab9-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15ab9-129">string</span></span> | <span data-ttu-id="15ab9-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="15ab9-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="15ab9-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="15ab9-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="15ab9-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="15ab9-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="15ab9-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15ab9-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="15ab9-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15ab9-134">Request headers</span></span>

| <span data-ttu-id="15ab9-135">Nome</span><span class="sxs-lookup"><span data-stu-id="15ab9-135">Name</span></span>          | <span data-ttu-id="15ab9-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ab9-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="15ab9-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="15ab9-137">Authorization</span></span> | <span data-ttu-id="15ab9-138">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="15ab9-138">Bearer {token}.</span></span> <span data-ttu-id="15ab9-139">Required.</span><span class="sxs-lookup"><span data-stu-id="15ab9-139">Required.</span></span>                |
| <span data-ttu-id="15ab9-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="15ab9-140">If-None-Match</span></span> | <span data-ttu-id="15ab9-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="15ab9-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="15ab9-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="15ab9-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="15ab9-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="15ab9-143">Response</span></span>

<span data-ttu-id="15ab9-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="15ab9-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="15ab9-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="15ab9-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="15ab9-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="15ab9-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="15ab9-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="15ab9-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="15ab9-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="15ab9-148">Report Refresh Date</span></span>
- <span data-ttu-id="15ab9-149">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="15ab9-149">Site Type</span></span>
- <span data-ttu-id="15ab9-150">Total</span><span class="sxs-lookup"><span data-stu-id="15ab9-150">Total</span></span>
- <span data-ttu-id="15ab9-151">Ativo</span><span class="sxs-lookup"><span data-stu-id="15ab9-151">Active</span></span>
- <span data-ttu-id="15ab9-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="15ab9-152">Report Date</span></span>
- <span data-ttu-id="15ab9-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="15ab9-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="15ab9-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15ab9-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="15ab9-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15ab9-155">Request</span></span>

<span data-ttu-id="15ab9-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="15ab9-156">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="15ab9-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="15ab9-157">Response</span></span>

<span data-ttu-id="15ab9-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15ab9-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="15ab9-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="15ab9-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
