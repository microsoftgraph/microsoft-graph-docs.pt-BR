---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Obtenha dados sobre o uso do dispositivo Skype for Business por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b422e5683f124d6a457402f0a554708d3e80fcbf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864261"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="ee30b-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="ee30b-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="ee30b-104">Obtenha dados sobre o uso do dispositivo Skype for Business por usuário.</span><span class="sxs-lookup"><span data-stu-id="ee30b-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="ee30b-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="ee30b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee30b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee30b-106">Permissions</span></span>

<span data-ttu-id="ee30b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee30b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee30b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee30b-109">Permission type</span></span>                        | <span data-ttu-id="ee30b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee30b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ee30b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee30b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee30b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee30b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ee30b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee30b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee30b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee30b-114">Not supported.</span></span>                           |
| <span data-ttu-id="ee30b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee30b-115">Application</span></span>                            | <span data-ttu-id="ee30b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee30b-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="ee30b-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="ee30b-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ee30b-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ee30b-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ee30b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee30b-119">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ee30b-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ee30b-120">Function parameters</span></span>

<span data-ttu-id="ee30b-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ee30b-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ee30b-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ee30b-122">Parameter</span></span> | <span data-ttu-id="ee30b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee30b-123">Type</span></span>   | <span data-ttu-id="ee30b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee30b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ee30b-125">ponto</span><span class="sxs-lookup"><span data-stu-id="ee30b-125">period</span></span>    | <span data-ttu-id="ee30b-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee30b-126">string</span></span> | <span data-ttu-id="ee30b-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ee30b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ee30b-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ee30b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ee30b-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ee30b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ee30b-130">data</span><span class="sxs-lookup"><span data-stu-id="ee30b-130">date</span></span>      | <span data-ttu-id="ee30b-131">Data</span><span class="sxs-lookup"><span data-stu-id="ee30b-131">Date</span></span>   | <span data-ttu-id="ee30b-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="ee30b-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ee30b-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="ee30b-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ee30b-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="ee30b-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ee30b-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="ee30b-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee30b-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee30b-136">Request headers</span></span>

| <span data-ttu-id="ee30b-137">Nome</span><span class="sxs-lookup"><span data-stu-id="ee30b-137">Name</span></span>          | <span data-ttu-id="ee30b-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee30b-138">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ee30b-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee30b-139">Authorization</span></span> | <span data-ttu-id="ee30b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee30b-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ee30b-142">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ee30b-142">If-None-Match</span></span> | <span data-ttu-id="ee30b-143">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="ee30b-143">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ee30b-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ee30b-144">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ee30b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee30b-145">Response</span></span>

<span data-ttu-id="ee30b-146">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ee30b-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ee30b-147">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ee30b-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ee30b-148">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ee30b-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ee30b-149">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ee30b-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ee30b-150">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ee30b-150">Report Refresh Date</span></span>
- <span data-ttu-id="ee30b-151">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="ee30b-151">User Principal Name</span></span>
- <span data-ttu-id="ee30b-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="ee30b-152">Last Activity Date</span></span>
- <span data-ttu-id="ee30b-153">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="ee30b-153">Used Windows</span></span>
- <span data-ttu-id="ee30b-154">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="ee30b-154">Used Windows Phone</span></span>
- <span data-ttu-id="ee30b-155">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="ee30b-155">Used Android Phone</span></span>
- <span data-ttu-id="ee30b-156">Usou iPhone</span><span class="sxs-lookup"><span data-stu-id="ee30b-156">Used iPhone</span></span>
- <span data-ttu-id="ee30b-157">Usou iPad</span><span class="sxs-lookup"><span data-stu-id="ee30b-157">Used iPad</span></span>
- <span data-ttu-id="ee30b-158">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ee30b-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ee30b-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee30b-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ee30b-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee30b-160">Request</span></span>

<span data-ttu-id="ee30b-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee30b-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ee30b-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee30b-162">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ee30b-163">C#</span><span class="sxs-lookup"><span data-stu-id="ee30b-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee30b-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee30b-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ee30b-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee30b-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ee30b-166">Java</span><span class="sxs-lookup"><span data-stu-id="ee30b-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ee30b-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee30b-167">Response</span></span>

<span data-ttu-id="ee30b-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ee30b-168">The following is an example of the response.</span></span>

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

<span data-ttu-id="ee30b-169">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ee30b-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
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
