---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a12e88a2011a98539b442b3321fb0c99b80b6726
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865248"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="61898-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="61898-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="61898-104">Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="61898-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="61898-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="61898-105">Permissions</span></span>

<span data-ttu-id="61898-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61898-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61898-108">Permission type</span></span>                        | <span data-ttu-id="61898-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61898-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="61898-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61898-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="61898-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="61898-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="61898-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61898-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61898-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61898-113">Not supported.</span></span>                           |
| <span data-ttu-id="61898-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61898-114">Application</span></span>                            | <span data-ttu-id="61898-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="61898-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="61898-116">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="61898-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="61898-117">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="61898-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="61898-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61898-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="61898-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="61898-119">Function parameters</span></span>

<span data-ttu-id="61898-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="61898-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="61898-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="61898-121">Parameter</span></span> | <span data-ttu-id="61898-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="61898-122">Type</span></span>   | <span data-ttu-id="61898-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="61898-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="61898-124">ponto</span><span class="sxs-lookup"><span data-stu-id="61898-124">period</span></span>    | <span data-ttu-id="61898-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61898-125">string</span></span> | <span data-ttu-id="61898-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="61898-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="61898-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="61898-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="61898-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="61898-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="61898-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61898-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="61898-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61898-130">Request headers</span></span>

| <span data-ttu-id="61898-131">Nome</span><span class="sxs-lookup"><span data-stu-id="61898-131">Name</span></span>          | <span data-ttu-id="61898-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="61898-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="61898-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="61898-133">Authorization</span></span> | <span data-ttu-id="61898-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61898-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="61898-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="61898-136">Response</span></span>

<span data-ttu-id="61898-137">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="61898-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="61898-138">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="61898-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="61898-139">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="61898-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="61898-140">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="61898-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="61898-141">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="61898-141">Report Refresh Date</span></span>
- <span data-ttu-id="61898-142">Web</span><span class="sxs-lookup"><span data-stu-id="61898-142">Web</span></span>
- <span data-ttu-id="61898-143">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="61898-143">Windows Phone</span></span>
- <span data-ttu-id="61898-144">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="61898-144">Android Phone</span></span>
- <span data-ttu-id="61898-145">iOS</span><span class="sxs-lookup"><span data-stu-id="61898-145">iOS</span></span>
- <span data-ttu-id="61898-146">Mac</span><span class="sxs-lookup"><span data-stu-id="61898-146">Mac</span></span>
- <span data-ttu-id="61898-147">Windows</span><span class="sxs-lookup"><span data-stu-id="61898-147">Windows</span></span>
- <span data-ttu-id="61898-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="61898-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="61898-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61898-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="61898-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61898-150">Request</span></span>

<span data-ttu-id="61898-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="61898-151">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="61898-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="61898-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="61898-153">C#</span><span class="sxs-lookup"><span data-stu-id="61898-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="61898-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61898-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="61898-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61898-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="61898-156">Java</span><span class="sxs-lookup"><span data-stu-id="61898-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusagedistributionusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="61898-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="61898-157">Response</span></span>

<span data-ttu-id="61898-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="61898-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="61898-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="61898-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
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
