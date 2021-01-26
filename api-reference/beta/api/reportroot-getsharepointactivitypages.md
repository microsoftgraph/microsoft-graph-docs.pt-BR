---
title: 'reportRoot: getSharePointActivityPages'
description: Obtenha o número de páginas exclusivas visitadas pelos usuários.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: d1a99b4bc0e621b9e1956dd0a7782e42d3c9dffa
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983311"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="3e7b2-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="3e7b2-103">reportRoot: getSharePointActivityPages</span></span>

<span data-ttu-id="3e7b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e7b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e7b2-105">Obtenha o número de páginas exclusivas visitadas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-105">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="3e7b2-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte [relatórios do Microsoft 365 - atividade do SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)</span><span class="sxs-lookup"><span data-stu-id="3e7b2-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e7b2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e7b2-107">Permissions</span></span>

<span data-ttu-id="3e7b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e7b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e7b2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e7b2-110">Permission type</span></span>                        | <span data-ttu-id="3e7b2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e7b2-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3e7b2-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e7b2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e7b2-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e7b2-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3e7b2-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e7b2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e7b2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-115">Not supported.</span></span>                           |
| <span data-ttu-id="3e7b2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e7b2-116">Application</span></span>                            | <span data-ttu-id="3e7b2-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e7b2-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="3e7b2-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3e7b2-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3e7b2-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3e7b2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e7b2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3e7b2-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3e7b2-121">Function parameters</span></span>

<span data-ttu-id="3e7b2-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3e7b2-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3e7b2-123">Parameter</span></span> | <span data-ttu-id="3e7b2-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e7b2-124">Type</span></span>   | <span data-ttu-id="3e7b2-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e7b2-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3e7b2-126">ponto</span><span class="sxs-lookup"><span data-stu-id="3e7b2-126">period</span></span>    | <span data-ttu-id="3e7b2-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e7b2-127">string</span></span> | <span data-ttu-id="3e7b2-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3e7b2-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3e7b2-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3e7b2-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-131">Required.</span></span> |

<span data-ttu-id="3e7b2-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3e7b2-133">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-133">The default output type is text/csv.</span></span> <span data-ttu-id="3e7b2-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e7b2-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e7b2-135">Request headers</span></span>

| <span data-ttu-id="3e7b2-136">Nome</span><span class="sxs-lookup"><span data-stu-id="3e7b2-136">Name</span></span>          | <span data-ttu-id="3e7b2-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e7b2-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3e7b2-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e7b2-138">Authorization</span></span> | <span data-ttu-id="3e7b2-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3e7b2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e7b2-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3e7b2-142">CSV</span><span class="sxs-lookup"><span data-stu-id="3e7b2-142">CSV</span></span>

<span data-ttu-id="3e7b2-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3e7b2-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3e7b2-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3e7b2-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3e7b2-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3e7b2-147">Report Refresh Date</span></span>
- <span data-ttu-id="3e7b2-148">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="3e7b2-148">Visited Page Count</span></span>
- <span data-ttu-id="3e7b2-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="3e7b2-149">Report Date</span></span>
- <span data-ttu-id="3e7b2-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="3e7b2-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3e7b2-151">JSON</span><span class="sxs-lookup"><span data-stu-id="3e7b2-151">JSON</span></span>

<span data-ttu-id="3e7b2-152">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` **[objeto sharePointActivityPages](../resources/sharepointactivitypages.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-152">If successful, this method returns a `200 OK` response code and a **[sharePointActivityPages](../resources/sharepointactivitypages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e7b2-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e7b2-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3e7b2-154">CSV</span><span class="sxs-lookup"><span data-stu-id="3e7b2-154">CSV</span></span>

<span data-ttu-id="3e7b2-155">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3e7b2-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e7b2-156">Request</span></span>

<span data-ttu-id="3e7b2-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-157">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivitypages_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="3e7b2-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e7b2-158">Response</span></span>

<span data-ttu-id="3e7b2-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3e7b2-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="3e7b2-161">JSON</span><span class="sxs-lookup"><span data-stu-id="3e7b2-161">JSON</span></span>

<span data-ttu-id="3e7b2-162">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3e7b2-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e7b2-163">Request</span></span>

<span data-ttu-id="3e7b2-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-164">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivitypages_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="3e7b2-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e7b2-165">Response</span></span>

<span data-ttu-id="3e7b2-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-166">The following is an example of the response.</span></span>

> <span data-ttu-id="3e7b2-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e7b2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityPages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPageCount": 195, 
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


