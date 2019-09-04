---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Obtenha o número de usuários diários por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 40e7c18f82dac1d02e0cfc9e119dab2c430c3cca
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729382"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="3aeab-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="3aeab-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="3aeab-104">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3aeab-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="3aeab-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="3aeab-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="3aeab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3aeab-106">Permissions</span></span>

<span data-ttu-id="3aeab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aeab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3aeab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3aeab-109">Permission type</span></span>                        | <span data-ttu-id="3aeab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3aeab-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3aeab-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3aeab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3aeab-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aeab-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3aeab-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3aeab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aeab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3aeab-114">Not supported.</span></span>                           |
| <span data-ttu-id="3aeab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3aeab-115">Application</span></span>                            | <span data-ttu-id="3aeab-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3aeab-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3aeab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3aeab-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3aeab-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3aeab-118">Function parameters</span></span>

<span data-ttu-id="3aeab-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3aeab-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3aeab-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3aeab-120">Parameter</span></span> | <span data-ttu-id="3aeab-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3aeab-121">Type</span></span>   | <span data-ttu-id="3aeab-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aeab-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3aeab-123">ponto</span><span class="sxs-lookup"><span data-stu-id="3aeab-123">period</span></span>    | <span data-ttu-id="3aeab-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3aeab-124">string</span></span> | <span data-ttu-id="3aeab-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3aeab-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3aeab-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3aeab-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3aeab-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3aeab-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3aeab-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3aeab-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3aeab-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3aeab-129">Request headers</span></span>

| <span data-ttu-id="3aeab-130">Nome</span><span class="sxs-lookup"><span data-stu-id="3aeab-130">Name</span></span>          | <span data-ttu-id="3aeab-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aeab-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3aeab-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="3aeab-132">Authorization</span></span> | <span data-ttu-id="3aeab-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3aeab-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3aeab-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3aeab-135">If-None-Match</span></span> | <span data-ttu-id="3aeab-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="3aeab-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3aeab-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3aeab-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3aeab-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aeab-138">Response</span></span>

<span data-ttu-id="3aeab-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3aeab-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3aeab-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3aeab-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3aeab-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3aeab-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3aeab-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3aeab-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3aeab-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3aeab-143">Report Refresh Date</span></span>
- <span data-ttu-id="3aeab-144">Web</span><span class="sxs-lookup"><span data-stu-id="3aeab-144">Web</span></span>
- <span data-ttu-id="3aeab-145">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="3aeab-145">Windows Phone</span></span>
- <span data-ttu-id="3aeab-146">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="3aeab-146">Android Phone</span></span>
- <span data-ttu-id="3aeab-147">iPhone</span><span class="sxs-lookup"><span data-stu-id="3aeab-147">iPhone</span></span>
- <span data-ttu-id="3aeab-148">iPad</span><span class="sxs-lookup"><span data-stu-id="3aeab-148">iPad</span></span>
- <span data-ttu-id="3aeab-149">Outro</span><span class="sxs-lookup"><span data-stu-id="3aeab-149">Other</span></span>
- <span data-ttu-id="3aeab-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="3aeab-150">Report Date</span></span>
- <span data-ttu-id="3aeab-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3aeab-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3aeab-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3aeab-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3aeab-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aeab-153">Request</span></span>

<span data-ttu-id="3aeab-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aeab-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3aeab-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aeab-155">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3aeab-156">C#</span><span class="sxs-lookup"><span data-stu-id="3aeab-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3aeab-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aeab-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3aeab-158">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3aeab-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3aeab-159">Java</span><span class="sxs-lookup"><span data-stu-id="3aeab-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3aeab-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aeab-160">Response</span></span>

<span data-ttu-id="3aeab-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3aeab-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="3aeab-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3aeab-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
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
