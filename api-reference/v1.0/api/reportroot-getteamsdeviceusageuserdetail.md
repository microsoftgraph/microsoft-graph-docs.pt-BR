---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d26096c5769ee94252163674764276f8735cd2ca
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458737"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="dd4a5-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="dd4a5-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="dd4a5-104">Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd4a5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd4a5-105">Permissions</span></span>

<span data-ttu-id="dd4a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd4a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd4a5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd4a5-108">Permission type</span></span>                        | <span data-ttu-id="dd4a5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd4a5-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dd4a5-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd4a5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd4a5-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd4a5-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dd4a5-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd4a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd4a5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-113">Not supported.</span></span>                           |
| <span data-ttu-id="dd4a5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd4a5-114">Application</span></span>                            | <span data-ttu-id="dd4a5-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd4a5-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dd4a5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd4a5-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="dd4a5-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="dd4a5-117">Function parameters</span></span>

<span data-ttu-id="dd4a5-118">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="dd4a5-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dd4a5-119">Parameter</span></span> | <span data-ttu-id="dd4a5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd4a5-120">Type</span></span>   | <span data-ttu-id="dd4a5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd4a5-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dd4a5-122">ponto</span><span class="sxs-lookup"><span data-stu-id="dd4a5-122">period</span></span>    | <span data-ttu-id="dd4a5-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd4a5-123">string</span></span> | <span data-ttu-id="dd4a5-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dd4a5-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dd4a5-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="dd4a5-127">data</span><span class="sxs-lookup"><span data-stu-id="dd4a5-127">date</span></span>      | <span data-ttu-id="dd4a5-128">Data</span><span class="sxs-lookup"><span data-stu-id="dd4a5-128">Date</span></span>   | <span data-ttu-id="dd4a5-129">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="dd4a5-130">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="dd4a5-131">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="dd4a5-132">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd4a5-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd4a5-133">Request headers</span></span>

| <span data-ttu-id="dd4a5-134">Nome</span><span class="sxs-lookup"><span data-stu-id="dd4a5-134">Name</span></span>          | <span data-ttu-id="dd4a5-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd4a5-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dd4a5-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd4a5-136">Authorization</span></span> | <span data-ttu-id="dd4a5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dd4a5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd4a5-139">Response</span></span>

<span data-ttu-id="dd4a5-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dd4a5-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dd4a5-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dd4a5-143">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="dd4a5-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="dd4a5-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="dd4a5-144">Report Refresh Date</span></span>
- <span data-ttu-id="dd4a5-145">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="dd4a5-145">User Principal Name</span></span>
- <span data-ttu-id="dd4a5-146">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="dd4a5-146">Last Activity Date</span></span>
- <span data-ttu-id="dd4a5-147">Excluído</span><span class="sxs-lookup"><span data-stu-id="dd4a5-147">Is Deleted</span></span>
- <span data-ttu-id="dd4a5-148">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="dd4a5-148">Deleted Date</span></span>
- <span data-ttu-id="dd4a5-149">Usou Web</span><span class="sxs-lookup"><span data-stu-id="dd4a5-149">Used Web</span></span>
- <span data-ttu-id="dd4a5-150">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="dd4a5-150">Used Windows Phone</span></span>
- <span data-ttu-id="dd4a5-151">Usou iOS</span><span class="sxs-lookup"><span data-stu-id="dd4a5-151">Used iOS</span></span>
- <span data-ttu-id="dd4a5-152">Usou Mac</span><span class="sxs-lookup"><span data-stu-id="dd4a5-152">Used Mac</span></span>
- <span data-ttu-id="dd4a5-153">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="dd4a5-153">Used Android Phone</span></span>
- <span data-ttu-id="dd4a5-154">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="dd4a5-154">Used Windows</span></span>
- <span data-ttu-id="dd4a5-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="dd4a5-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="dd4a5-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd4a5-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dd4a5-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd4a5-157">Request</span></span>

<span data-ttu-id="dd4a5-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dd4a5-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd4a5-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd4a5-160">C#</span><span class="sxs-lookup"><span data-stu-id="dd4a5-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd4a5-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="dd4a5-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd4a5-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dd4a5-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dd4a5-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd4a5-163">Response</span></span>

<span data-ttu-id="dd4a5-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="dd4a5-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="dd4a5-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
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
