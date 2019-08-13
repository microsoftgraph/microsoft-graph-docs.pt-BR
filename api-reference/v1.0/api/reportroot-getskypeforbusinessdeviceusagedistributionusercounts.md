---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Obtenha o número de usuários que usam dispositivos exclusivos em sua organização. O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9f88aad9461fafe561c4b1b7b2801f3c7b8012f0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349171"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="866e5-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="866e5-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="866e5-105">Obtenha o número de usuários que usam dispositivos exclusivos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="866e5-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="866e5-106">O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.</span><span class="sxs-lookup"><span data-stu-id="866e5-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="866e5-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="866e5-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="866e5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="866e5-108">Permissions</span></span>

<span data-ttu-id="866e5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="866e5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="866e5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="866e5-111">Permission type</span></span>                        | <span data-ttu-id="866e5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="866e5-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="866e5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="866e5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="866e5-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="866e5-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="866e5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="866e5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="866e5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="866e5-116">Not supported.</span></span>                           |
| <span data-ttu-id="866e5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="866e5-117">Application</span></span>                            | <span data-ttu-id="866e5-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="866e5-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="866e5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="866e5-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="866e5-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="866e5-120">Function parameters</span></span>

<span data-ttu-id="866e5-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="866e5-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="866e5-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="866e5-122">Parameter</span></span> | <span data-ttu-id="866e5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="866e5-123">Type</span></span>   | <span data-ttu-id="866e5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="866e5-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="866e5-125">ponto</span><span class="sxs-lookup"><span data-stu-id="866e5-125">period</span></span>    | <span data-ttu-id="866e5-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="866e5-126">string</span></span> | <span data-ttu-id="866e5-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="866e5-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="866e5-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="866e5-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="866e5-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="866e5-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="866e5-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="866e5-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="866e5-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="866e5-131">Request headers</span></span>

| <span data-ttu-id="866e5-132">Nome</span><span class="sxs-lookup"><span data-stu-id="866e5-132">Name</span></span>          | <span data-ttu-id="866e5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="866e5-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="866e5-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="866e5-134">Authorization</span></span> | <span data-ttu-id="866e5-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="866e5-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="866e5-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="866e5-137">If-None-Match</span></span> | <span data-ttu-id="866e5-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="866e5-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="866e5-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="866e5-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="866e5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="866e5-140">Response</span></span>

<span data-ttu-id="866e5-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="866e5-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="866e5-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="866e5-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="866e5-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="866e5-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="866e5-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="866e5-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="866e5-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="866e5-145">Report Refresh Date</span></span>
- <span data-ttu-id="866e5-146">Windows</span><span class="sxs-lookup"><span data-stu-id="866e5-146">Windows</span></span>
- <span data-ttu-id="866e5-147">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="866e5-147">Windows Phone</span></span>
- <span data-ttu-id="866e5-148">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="866e5-148">Android Phone</span></span>
- <span data-ttu-id="866e5-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="866e5-149">iPhone</span></span>
- <span data-ttu-id="866e5-150">iPad</span><span class="sxs-lookup"><span data-stu-id="866e5-150">iPad</span></span>
- <span data-ttu-id="866e5-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="866e5-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="866e5-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="866e5-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="866e5-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="866e5-153">Request</span></span>

<span data-ttu-id="866e5-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="866e5-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="866e5-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="866e5-155">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="866e5-156">C#</span><span class="sxs-lookup"><span data-stu-id="866e5-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="866e5-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="866e5-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="866e5-158">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="866e5-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="866e5-159">Java</span><span class="sxs-lookup"><span data-stu-id="866e5-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="866e5-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="866e5-160">Response</span></span>

<span data-ttu-id="866e5-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="866e5-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="866e5-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="866e5-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
