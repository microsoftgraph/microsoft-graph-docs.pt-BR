---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Obtenha a contagem de usuários ativos diários no período de relatório por produto.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 2b155d27a0c32f934b6e5ea980f5ba85a5c8c652
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053528"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="5bcbf-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="5bcbf-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="5bcbf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bcbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bcbf-105">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-105">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="5bcbf-106">**Observação:** Para saber mais sobre os diferentes modos de exibição de relatório e nomes, confira [Relatórios do Microsoft 365 - Usuários Ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d). </span><span class="sxs-lookup"><span data-stu-id="5bcbf-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="5bcbf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5bcbf-107">Permissions</span></span>

<span data-ttu-id="5bcbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bcbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5bcbf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bcbf-110">Permission type</span></span>                        | <span data-ttu-id="5bcbf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bcbf-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5bcbf-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bcbf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5bcbf-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bcbf-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5bcbf-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bcbf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bcbf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-115">Not supported.</span></span>                           |
| <span data-ttu-id="5bcbf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bcbf-116">Application</span></span>                            | <span data-ttu-id="5bcbf-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bcbf-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="5bcbf-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5bcbf-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5bcbf-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5bcbf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bcbf-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5bcbf-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5bcbf-121">Function parameters</span></span>

<span data-ttu-id="5bcbf-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5bcbf-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5bcbf-123">Parameter</span></span> | <span data-ttu-id="5bcbf-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bcbf-124">Type</span></span>   | <span data-ttu-id="5bcbf-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bcbf-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5bcbf-126">ponto</span><span class="sxs-lookup"><span data-stu-id="5bcbf-126">period</span></span>    | <span data-ttu-id="5bcbf-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bcbf-127">string</span></span> | <span data-ttu-id="5bcbf-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5bcbf-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5bcbf-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5bcbf-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-131">Required.</span></span> |

<span data-ttu-id="5bcbf-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5bcbf-133">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-133">The default output type is text/csv.</span></span> <span data-ttu-id="5bcbf-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bcbf-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bcbf-135">Request headers</span></span>

| <span data-ttu-id="5bcbf-136">Nome</span><span class="sxs-lookup"><span data-stu-id="5bcbf-136">Name</span></span>          | <span data-ttu-id="5bcbf-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bcbf-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5bcbf-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bcbf-138">Authorization</span></span> | <span data-ttu-id="5bcbf-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5bcbf-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bcbf-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5bcbf-142">CSV</span><span class="sxs-lookup"><span data-stu-id="5bcbf-142">CSV</span></span>

<span data-ttu-id="5bcbf-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5bcbf-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5bcbf-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5bcbf-146">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="5bcbf-146">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="5bcbf-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5bcbf-147">Report Refresh Date</span></span>
- <span data-ttu-id="5bcbf-148">Office 365</span><span class="sxs-lookup"><span data-stu-id="5bcbf-148">Office 365</span></span>
- <span data-ttu-id="5bcbf-149">Exchange</span><span class="sxs-lookup"><span data-stu-id="5bcbf-149">Exchange</span></span>
- <span data-ttu-id="5bcbf-150">OneDrive</span><span class="sxs-lookup"><span data-stu-id="5bcbf-150">OneDrive</span></span>
- <span data-ttu-id="5bcbf-151">SharePoint</span><span class="sxs-lookup"><span data-stu-id="5bcbf-151">SharePoint</span></span>
- <span data-ttu-id="5bcbf-152">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="5bcbf-152">Skype For Business</span></span> 
- <span data-ttu-id="5bcbf-153">Yammer</span><span class="sxs-lookup"><span data-stu-id="5bcbf-153">Yammer</span></span>
- <span data-ttu-id="5bcbf-154">Teams</span><span class="sxs-lookup"><span data-stu-id="5bcbf-154">Teams</span></span>
- <span data-ttu-id="5bcbf-155">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="5bcbf-155">Report Date</span></span>
- <span data-ttu-id="5bcbf-156">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5bcbf-156">Report Period</span></span>

<span data-ttu-id="5bcbf-157">As seguintes colunas não são suportadas na Microsoft Graph China operada pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="5bcbf-157">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="5bcbf-158">Yammer</span><span class="sxs-lookup"><span data-stu-id="5bcbf-158">Yammer</span></span>
- <span data-ttu-id="5bcbf-159">Teams</span><span class="sxs-lookup"><span data-stu-id="5bcbf-159">Teams</span></span>

### <a name="json"></a><span data-ttu-id="5bcbf-160">JSON</span><span class="sxs-lookup"><span data-stu-id="5bcbf-160">JSON</span></span>

<span data-ttu-id="5bcbf-161">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto office365ActiveUserCounts](../resources/office365activeusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-161">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="5bcbf-162">As seguintes propriedades no **[objeto office365ActiveUserCounts](../resources/office365activeusercounts.md)** não são suportadas no Microsoft Graph China operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="5bcbf-162">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="5bcbf-163">yammer</span><span class="sxs-lookup"><span data-stu-id="5bcbf-163">yammer</span></span>
- <span data-ttu-id="5bcbf-164">teams</span><span class="sxs-lookup"><span data-stu-id="5bcbf-164">teams</span></span>

## <a name="example"></a><span data-ttu-id="5bcbf-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bcbf-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5bcbf-166">CSV</span><span class="sxs-lookup"><span data-stu-id="5bcbf-166">CSV</span></span>

<span data-ttu-id="5bcbf-167">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5bcbf-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bcbf-168">Request</span></span>

<span data-ttu-id="5bcbf-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="5bcbf-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bcbf-170">Response</span></span>

<span data-ttu-id="5bcbf-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5bcbf-172">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="5bcbf-173">JSON</span><span class="sxs-lookup"><span data-stu-id="5bcbf-173">JSON</span></span>

<span data-ttu-id="5bcbf-174">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5bcbf-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bcbf-175">Request</span></span>

<span data-ttu-id="5bcbf-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-176">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="5bcbf-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bcbf-177">Response</span></span>

<span data-ttu-id="5bcbf-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-178">The following is an example of the response.</span></span>

> <span data-ttu-id="5bcbf-179">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5bcbf-179">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
      "reportPeriod": "7"
    }
  ]
}
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


