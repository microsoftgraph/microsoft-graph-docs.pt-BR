---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: bad7ac5299795ee69108dd14af9a11a0ab332662
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864240"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="e01ea-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="e01ea-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="e01ea-104">Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="e01ea-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="e01ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e01ea-105">Permissions</span></span>

<span data-ttu-id="e01ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e01ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e01ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e01ea-108">Permission type</span></span>                        | <span data-ttu-id="e01ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e01ea-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e01ea-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e01ea-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e01ea-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e01ea-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e01ea-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e01ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e01ea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e01ea-113">Not supported.</span></span>                           |
| <span data-ttu-id="e01ea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e01ea-114">Application</span></span>                            | <span data-ttu-id="e01ea-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e01ea-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="e01ea-116">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="e01ea-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e01ea-117">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="e01ea-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e01ea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e01ea-118">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e01ea-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e01ea-119">Function parameters</span></span>

<span data-ttu-id="e01ea-120">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e01ea-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e01ea-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e01ea-121">Parameter</span></span> | <span data-ttu-id="e01ea-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e01ea-122">Type</span></span>   | <span data-ttu-id="e01ea-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e01ea-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e01ea-124">ponto</span><span class="sxs-lookup"><span data-stu-id="e01ea-124">period</span></span>    | <span data-ttu-id="e01ea-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e01ea-125">string</span></span> | <span data-ttu-id="e01ea-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e01ea-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e01ea-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e01ea-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e01ea-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e01ea-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e01ea-129">data</span><span class="sxs-lookup"><span data-stu-id="e01ea-129">date</span></span>      | <span data-ttu-id="e01ea-130">Data</span><span class="sxs-lookup"><span data-stu-id="e01ea-130">Date</span></span>   | <span data-ttu-id="e01ea-131">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="e01ea-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e01ea-132">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="e01ea-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e01ea-133">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="e01ea-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e01ea-134">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="e01ea-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e01ea-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e01ea-135">Request headers</span></span>

| <span data-ttu-id="e01ea-136">Nome</span><span class="sxs-lookup"><span data-stu-id="e01ea-136">Name</span></span>          | <span data-ttu-id="e01ea-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="e01ea-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e01ea-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="e01ea-138">Authorization</span></span> | <span data-ttu-id="e01ea-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e01ea-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e01ea-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e01ea-141">Response</span></span>

<span data-ttu-id="e01ea-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e01ea-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e01ea-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e01ea-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e01ea-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e01ea-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e01ea-145">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="e01ea-145">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="e01ea-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e01ea-146">Report Refresh Date</span></span>
- <span data-ttu-id="e01ea-147">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="e01ea-147">User Principal Name</span></span>
- <span data-ttu-id="e01ea-148">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="e01ea-148">Last Activity Date</span></span>
- <span data-ttu-id="e01ea-149">Excluído</span><span class="sxs-lookup"><span data-stu-id="e01ea-149">Is Deleted</span></span>
- <span data-ttu-id="e01ea-150">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="e01ea-150">Deleted Date</span></span>
- <span data-ttu-id="e01ea-151">Usou Web</span><span class="sxs-lookup"><span data-stu-id="e01ea-151">Used Web</span></span>
- <span data-ttu-id="e01ea-152">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="e01ea-152">Used Windows Phone</span></span>
- <span data-ttu-id="e01ea-153">Usou iOS</span><span class="sxs-lookup"><span data-stu-id="e01ea-153">Used iOS</span></span>
- <span data-ttu-id="e01ea-154">Usou Mac</span><span class="sxs-lookup"><span data-stu-id="e01ea-154">Used Mac</span></span>
- <span data-ttu-id="e01ea-155">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="e01ea-155">Used Android Phone</span></span>
- <span data-ttu-id="e01ea-156">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="e01ea-156">Used Windows</span></span>
- <span data-ttu-id="e01ea-157">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e01ea-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e01ea-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e01ea-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e01ea-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e01ea-159">Request</span></span>

<span data-ttu-id="e01ea-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e01ea-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e01ea-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="e01ea-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e01ea-162">C#</span><span class="sxs-lookup"><span data-stu-id="e01ea-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e01ea-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e01ea-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e01ea-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e01ea-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e01ea-165">Java</span><span class="sxs-lookup"><span data-stu-id="e01ea-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e01ea-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="e01ea-166">Response</span></span>

<span data-ttu-id="e01ea-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e01ea-167">The following is an example of the response.</span></span>

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

<span data-ttu-id="e01ea-168">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e01ea-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
