---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Obtenha o número de usuários que usam dispositivos exclusivos em sua organização. O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8fbd031f91fba63069cac3a16595d3f46bc8ea8b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892457"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="65651-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="65651-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="65651-105">Obtenha o número de usuários que usam dispositivos exclusivos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="65651-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="65651-106">O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.</span><span class="sxs-lookup"><span data-stu-id="65651-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="65651-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="65651-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="65651-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="65651-108">Permissions</span></span>

<span data-ttu-id="65651-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65651-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65651-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65651-111">Permission type</span></span>                        | <span data-ttu-id="65651-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65651-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="65651-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65651-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="65651-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65651-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="65651-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65651-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65651-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65651-116">Not supported.</span></span>                           |
| <span data-ttu-id="65651-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65651-117">Application</span></span>                            | <span data-ttu-id="65651-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65651-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="65651-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65651-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="65651-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="65651-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="65651-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="65651-121">Function parameters</span></span>

<span data-ttu-id="65651-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="65651-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="65651-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="65651-123">Parameter</span></span> | <span data-ttu-id="65651-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="65651-124">Type</span></span>   | <span data-ttu-id="65651-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="65651-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="65651-126">ponto</span><span class="sxs-lookup"><span data-stu-id="65651-126">period</span></span>    | <span data-ttu-id="65651-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65651-127">string</span></span> | <span data-ttu-id="65651-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="65651-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="65651-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="65651-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="65651-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="65651-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="65651-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65651-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="65651-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65651-132">Request headers</span></span>

| <span data-ttu-id="65651-133">Nome</span><span class="sxs-lookup"><span data-stu-id="65651-133">Name</span></span>          | <span data-ttu-id="65651-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="65651-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="65651-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="65651-135">Authorization</span></span> | <span data-ttu-id="65651-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65651-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="65651-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="65651-138">If-None-Match</span></span> | <span data-ttu-id="65651-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="65651-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="65651-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="65651-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="65651-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="65651-141">Response</span></span>

<span data-ttu-id="65651-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="65651-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="65651-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="65651-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="65651-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="65651-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="65651-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="65651-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="65651-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="65651-146">Report Refresh Date</span></span>
- <span data-ttu-id="65651-147">Windows</span><span class="sxs-lookup"><span data-stu-id="65651-147">Windows</span></span>
- <span data-ttu-id="65651-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="65651-148">Windows Phone</span></span>
- <span data-ttu-id="65651-149">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="65651-149">Android Phone</span></span>
- <span data-ttu-id="65651-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="65651-150">iPhone</span></span>
- <span data-ttu-id="65651-151">iPad</span><span class="sxs-lookup"><span data-stu-id="65651-151">iPad</span></span>
- <span data-ttu-id="65651-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="65651-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="65651-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65651-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="65651-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65651-154">Request</span></span>

<span data-ttu-id="65651-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="65651-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65651-156">C#</span><span class="sxs-lookup"><span data-stu-id="65651-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65651-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="65651-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65651-158">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="65651-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65651-159">Java</span><span class="sxs-lookup"><span data-stu-id="65651-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65651-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="65651-160">Response</span></span>

<span data-ttu-id="65651-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="65651-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="65651-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="65651-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
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
