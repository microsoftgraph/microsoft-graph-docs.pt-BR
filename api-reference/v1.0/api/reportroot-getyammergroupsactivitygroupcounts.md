---
title: 'reportRoot: getYammerGroupsActivityGroupCounts'
description: Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7a825f554f3eb9418b06dccd37a110b75f761b67
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864156"
---
# <a name="reportroot-getyammergroupsactivitygroupcounts"></a><span data-ttu-id="44748-103">reportRoot: getYammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="44748-103">reportRoot: getYammerGroupsActivityGroupCounts</span></span>

<span data-ttu-id="44748-104">Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo.</span><span class="sxs-lookup"><span data-stu-id="44748-104">Get the total number of groups that existed and how many included group conversation activity.</span></span>

> <span data-ttu-id="44748-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="44748-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="44748-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="44748-106">Permissions</span></span>

<span data-ttu-id="44748-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44748-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44748-109">Permission type</span></span>                        | <span data-ttu-id="44748-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44748-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="44748-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44748-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="44748-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44748-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="44748-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44748-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44748-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44748-114">Not supported.</span></span>                           |
| <span data-ttu-id="44748-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44748-115">Application</span></span>                            | <span data-ttu-id="44748-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44748-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="44748-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="44748-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="44748-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="44748-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="44748-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44748-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="44748-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="44748-120">Function parameters</span></span>

<span data-ttu-id="44748-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="44748-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="44748-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="44748-122">Parameter</span></span> | <span data-ttu-id="44748-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="44748-123">Type</span></span>   | <span data-ttu-id="44748-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="44748-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="44748-125">ponto</span><span class="sxs-lookup"><span data-stu-id="44748-125">period</span></span>    | <span data-ttu-id="44748-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44748-126">string</span></span> | <span data-ttu-id="44748-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="44748-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="44748-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="44748-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="44748-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="44748-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="44748-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44748-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="44748-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44748-131">Request headers</span></span>

| <span data-ttu-id="44748-132">Nome</span><span class="sxs-lookup"><span data-stu-id="44748-132">Name</span></span>          | <span data-ttu-id="44748-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="44748-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="44748-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="44748-134">Authorization</span></span> | <span data-ttu-id="44748-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44748-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="44748-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="44748-137">If-None-Match</span></span> | <span data-ttu-id="44748-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="44748-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="44748-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="44748-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="44748-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="44748-140">Response</span></span>

<span data-ttu-id="44748-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="44748-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="44748-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="44748-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="44748-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="44748-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="44748-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="44748-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="44748-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="44748-145">Report Refresh Date</span></span>
- <span data-ttu-id="44748-146">Total</span><span class="sxs-lookup"><span data-stu-id="44748-146">Total</span></span>
- <span data-ttu-id="44748-147">Ativo</span><span class="sxs-lookup"><span data-stu-id="44748-147">Active</span></span>
- <span data-ttu-id="44748-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="44748-148">Report Date</span></span>
- <span data-ttu-id="44748-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="44748-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="44748-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44748-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="44748-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44748-151">Request</span></span>

<span data-ttu-id="44748-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="44748-152">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="44748-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="44748-153">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivitygroupcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityGroupCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44748-154">C#</span><span class="sxs-lookup"><span data-stu-id="44748-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitygroupcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44748-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44748-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitygroupcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44748-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44748-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitygroupcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="44748-157">Java</span><span class="sxs-lookup"><span data-stu-id="44748-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivitygroupcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44748-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="44748-158">Response</span></span>

<span data-ttu-id="44748-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="44748-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="44748-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="44748-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
