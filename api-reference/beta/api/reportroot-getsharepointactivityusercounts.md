---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 1a0ab92c3713934901372d9490d81034a783b3dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454259"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="c345b-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="c345b-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="c345b-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c345b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c345b-106">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="c345b-106">Get the trend in the number of active users.</span></span> <span data-ttu-id="c345b-107">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="c345b-107">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="c345b-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="c345b-108">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="c345b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c345b-109">Permissions</span></span>

<span data-ttu-id="c345b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c345b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c345b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c345b-112">Permission type</span></span>                        | <span data-ttu-id="c345b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c345b-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c345b-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c345b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c345b-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c345b-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c345b-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c345b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c345b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c345b-117">Not supported.</span></span>                           |
| <span data-ttu-id="c345b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c345b-118">Application</span></span>                            | <span data-ttu-id="c345b-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c345b-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="c345b-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="c345b-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="c345b-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="c345b-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="c345b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c345b-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c345b-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c345b-123">Function parameters</span></span>

<span data-ttu-id="c345b-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="c345b-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c345b-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c345b-125">Parameter</span></span> | <span data-ttu-id="c345b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="c345b-126">Type</span></span>   | <span data-ttu-id="c345b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c345b-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c345b-128">ponto</span><span class="sxs-lookup"><span data-stu-id="c345b-128">period</span></span>    | <span data-ttu-id="c345b-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c345b-129">string</span></span> | <span data-ttu-id="c345b-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c345b-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c345b-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="c345b-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c345b-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c345b-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c345b-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c345b-133">Required.</span></span> |

<span data-ttu-id="c345b-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c345b-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c345b-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="c345b-135">The default output type is text/csv.</span></span> <span data-ttu-id="c345b-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c345b-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c345b-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c345b-137">Request headers</span></span>

| <span data-ttu-id="c345b-138">Nome</span><span class="sxs-lookup"><span data-stu-id="c345b-138">Name</span></span>          | <span data-ttu-id="c345b-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="c345b-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c345b-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="c345b-140">Authorization</span></span> | <span data-ttu-id="c345b-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c345b-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c345b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c345b-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c345b-144">CSV</span><span class="sxs-lookup"><span data-stu-id="c345b-144">CSV</span></span>

<span data-ttu-id="c345b-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="c345b-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c345b-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c345b-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c345b-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c345b-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c345b-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="c345b-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c345b-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="c345b-149">Report Refresh Date</span></span>
- <span data-ttu-id="c345b-150">Página visitada</span><span class="sxs-lookup"><span data-stu-id="c345b-150">Visited Page</span></span>
- <span data-ttu-id="c345b-151">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="c345b-151">Viewed Or Edited</span></span>
- <span data-ttu-id="c345b-152">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="c345b-152">Synced</span></span>
- <span data-ttu-id="c345b-153">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="c345b-153">Shared Internally</span></span>
- <span data-ttu-id="c345b-154">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="c345b-154">Shared Externally</span></span>
- <span data-ttu-id="c345b-155">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="c345b-155">Report Date</span></span>
- <span data-ttu-id="c345b-156">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="c345b-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c345b-157">JSON</span><span class="sxs-lookup"><span data-stu-id="c345b-157">JSON</span></span>

<span data-ttu-id="c345b-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c345b-158">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c345b-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c345b-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c345b-160">CSV</span><span class="sxs-lookup"><span data-stu-id="c345b-160">CSV</span></span>

<span data-ttu-id="c345b-161">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="c345b-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c345b-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c345b-162">Request</span></span>

<span data-ttu-id="c345b-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c345b-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c345b-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="c345b-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="c345b-165">C#</span><span class="sxs-lookup"><span data-stu-id="c345b-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c345b-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c345b-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c345b-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c345b-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c345b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c345b-168">Response</span></span>

<span data-ttu-id="c345b-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c345b-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c345b-170">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="c345b-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="c345b-171">JSON</span><span class="sxs-lookup"><span data-stu-id="c345b-171">JSON</span></span>

<span data-ttu-id="c345b-172">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="c345b-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c345b-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c345b-173">Request</span></span>

<span data-ttu-id="c345b-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c345b-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c345b-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="c345b-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="c345b-176">C#</span><span class="sxs-lookup"><span data-stu-id="c345b-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c345b-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c345b-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c345b-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c345b-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c345b-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="c345b-179">Response</span></span>

<span data-ttu-id="c345b-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c345b-180">The following is an example of the response.</span></span>

> <span data-ttu-id="c345b-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c345b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
      "reportDate": "2017-09-01", 
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
