---
title: 'reportRoot: getOffice365GroupsActivityFileCounts'
description: Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2560472cec0d26099875c9e9950a5bfcf86e1159
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728157"
---
# <a name="reportroot-getoffice365groupsactivityfilecounts"></a><span data-ttu-id="32985-103">reportRoot: getOffice365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="32985-103">reportRoot: getOffice365GroupsActivityFileCounts</span></span>

<span data-ttu-id="32985-104">Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="32985-104">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span>

> <span data-ttu-id="32985-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="32985-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="32985-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="32985-106">Permissions</span></span>

<span data-ttu-id="32985-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32985-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32985-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32985-109">Permission type</span></span>                        | <span data-ttu-id="32985-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32985-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="32985-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32985-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="32985-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32985-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="32985-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32985-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32985-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32985-114">Not supported.</span></span>                           |
| <span data-ttu-id="32985-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32985-115">Application</span></span>                            | <span data-ttu-id="32985-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="32985-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="32985-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32985-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="32985-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="32985-118">Function parameters</span></span>

<span data-ttu-id="32985-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="32985-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="32985-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="32985-120">Parameter</span></span> | <span data-ttu-id="32985-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="32985-121">Type</span></span>   | <span data-ttu-id="32985-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="32985-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="32985-123">ponto</span><span class="sxs-lookup"><span data-stu-id="32985-123">period</span></span>    | <span data-ttu-id="32985-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32985-124">string</span></span> | <span data-ttu-id="32985-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="32985-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="32985-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="32985-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="32985-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="32985-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="32985-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32985-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="32985-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32985-129">Request headers</span></span>

| <span data-ttu-id="32985-130">Nome</span><span class="sxs-lookup"><span data-stu-id="32985-130">Name</span></span>          | <span data-ttu-id="32985-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="32985-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="32985-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="32985-132">Authorization</span></span> | <span data-ttu-id="32985-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32985-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="32985-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="32985-135">If-None-Match</span></span> | <span data-ttu-id="32985-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="32985-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="32985-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="32985-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="32985-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="32985-138">Response</span></span>

<span data-ttu-id="32985-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="32985-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="32985-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="32985-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="32985-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="32985-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="32985-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="32985-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="32985-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="32985-143">Report Refresh Date</span></span>
- <span data-ttu-id="32985-144">Total</span><span class="sxs-lookup"><span data-stu-id="32985-144">Total</span></span>
- <span data-ttu-id="32985-145">Ativo</span><span class="sxs-lookup"><span data-stu-id="32985-145">Active</span></span>
- <span data-ttu-id="32985-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="32985-146">Report Date</span></span>
- <span data-ttu-id="32985-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="32985-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="32985-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32985-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="32985-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32985-149">Request</span></span>

<span data-ttu-id="32985-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="32985-150">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="32985-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="32985-151">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityfilecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityFileCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="32985-152">C#</span><span class="sxs-lookup"><span data-stu-id="32985-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityfilecounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32985-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32985-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityfilecounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="32985-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="32985-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityfilecounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="32985-155">Java</span><span class="sxs-lookup"><span data-stu-id="32985-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivityfilecounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="32985-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="32985-156">Response</span></span>

<span data-ttu-id="32985-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="32985-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="32985-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="32985-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
