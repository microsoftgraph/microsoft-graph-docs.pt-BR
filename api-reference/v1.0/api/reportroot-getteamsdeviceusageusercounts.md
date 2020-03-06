---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Obtém o número de usuários exclusivos diários do Microsoft Teams por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d883ed329ed7cda602003cb4f84ee509254bc10a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510071"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="cb956-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="cb956-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="cb956-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb956-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb956-105">Obtém o número de usuários exclusivos diários do Microsoft Teams por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cb956-105">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb956-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb956-106">Permissions</span></span>

<span data-ttu-id="cb956-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb956-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb956-109">Permission type</span></span>                        | <span data-ttu-id="cb956-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb956-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cb956-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb956-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb956-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb956-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cb956-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb956-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb956-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb956-114">Not supported.</span></span>                           |
| <span data-ttu-id="cb956-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb956-115">Application</span></span>                            | <span data-ttu-id="cb956-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb956-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="cb956-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="cb956-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="cb956-118">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="cb956-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="cb956-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb956-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cb956-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="cb956-120">Function parameters</span></span>

<span data-ttu-id="cb956-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="cb956-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cb956-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cb956-122">Parameter</span></span> | <span data-ttu-id="cb956-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb956-123">Type</span></span>   | <span data-ttu-id="cb956-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb956-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cb956-125">ponto</span><span class="sxs-lookup"><span data-stu-id="cb956-125">period</span></span>    | <span data-ttu-id="cb956-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb956-126">string</span></span> | <span data-ttu-id="cb956-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cb956-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cb956-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="cb956-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cb956-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="cb956-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cb956-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb956-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="cb956-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb956-131">Request headers</span></span>

| <span data-ttu-id="cb956-132">Nome</span><span class="sxs-lookup"><span data-stu-id="cb956-132">Name</span></span>          | <span data-ttu-id="cb956-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb956-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cb956-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb956-134">Authorization</span></span> | <span data-ttu-id="cb956-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb956-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cb956-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb956-137">Response</span></span>

<span data-ttu-id="cb956-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="cb956-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cb956-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="cb956-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cb956-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cb956-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cb956-141">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="cb956-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="cb956-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="cb956-142">Report Refresh Date</span></span>
- <span data-ttu-id="cb956-143">Web</span><span class="sxs-lookup"><span data-stu-id="cb956-143">Web</span></span>
- <span data-ttu-id="cb956-144">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="cb956-144">Windows Phone</span></span>
- <span data-ttu-id="cb956-145">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="cb956-145">Android Phone</span></span>
- <span data-ttu-id="cb956-146">iOS</span><span class="sxs-lookup"><span data-stu-id="cb956-146">iOS</span></span>
- <span data-ttu-id="cb956-147">Mac</span><span class="sxs-lookup"><span data-stu-id="cb956-147">Mac</span></span>
- <span data-ttu-id="cb956-148">Windows</span><span class="sxs-lookup"><span data-stu-id="cb956-148">Windows</span></span>
- <span data-ttu-id="cb956-149">Data do Relatório</span><span class="sxs-lookup"><span data-stu-id="cb956-149">Report Date</span></span>
- <span data-ttu-id="cb956-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="cb956-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="cb956-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb956-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cb956-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb956-152">Request</span></span>

<span data-ttu-id="cb956-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb956-153">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cb956-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb956-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="cb956-155">C#</span><span class="sxs-lookup"><span data-stu-id="cb956-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb956-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb956-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb956-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb956-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb956-158">Java</span><span class="sxs-lookup"><span data-stu-id="cb956-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cb956-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb956-159">Response</span></span>

<span data-ttu-id="cb956-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cb956-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="cb956-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="cb956-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
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
