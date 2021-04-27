---
title: 'reportRoot: getYammerActivityUserCounts'
description: Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: eb1b80b55a93ccc2eff61fc8eb5ec9046d890f2e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054977"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="11921-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="11921-103">reportRoot: getYammerActivityUserCounts</span></span>

<span data-ttu-id="11921-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11921-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11921-105">Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="11921-105">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="11921-106">**Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Yammer Atividade](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="11921-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="11921-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="11921-107">Permissions</span></span>

<span data-ttu-id="11921-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11921-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11921-110">Permission type</span></span>                        | <span data-ttu-id="11921-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11921-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="11921-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11921-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="11921-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11921-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="11921-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11921-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11921-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11921-115">Not supported.</span></span>                           |
| <span data-ttu-id="11921-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11921-116">Application</span></span>                            | <span data-ttu-id="11921-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="11921-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="11921-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="11921-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="11921-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="11921-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="11921-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11921-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="11921-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="11921-121">Function parameters</span></span>

<span data-ttu-id="11921-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="11921-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="11921-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="11921-123">Parameter</span></span> | <span data-ttu-id="11921-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="11921-124">Type</span></span>   | <span data-ttu-id="11921-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="11921-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="11921-126">ponto</span><span class="sxs-lookup"><span data-stu-id="11921-126">period</span></span>    | <span data-ttu-id="11921-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11921-127">string</span></span> | <span data-ttu-id="11921-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="11921-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="11921-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="11921-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="11921-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="11921-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="11921-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11921-131">Required.</span></span> |

<span data-ttu-id="11921-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="11921-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="11921-133">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="11921-133">The default output type is text/csv.</span></span> <span data-ttu-id="11921-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="11921-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11921-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11921-135">Request headers</span></span>

| <span data-ttu-id="11921-136">Nome</span><span class="sxs-lookup"><span data-stu-id="11921-136">Name</span></span>          | <span data-ttu-id="11921-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="11921-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="11921-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="11921-138">Authorization</span></span> | <span data-ttu-id="11921-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11921-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="11921-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="11921-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="11921-142">CSV</span><span class="sxs-lookup"><span data-stu-id="11921-142">CSV</span></span>

<span data-ttu-id="11921-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="11921-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="11921-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="11921-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="11921-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="11921-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="11921-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="11921-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="11921-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="11921-147">Report Refresh Date</span></span>
- <span data-ttu-id="11921-148">Curtidos</span><span class="sxs-lookup"><span data-stu-id="11921-148">Liked</span></span>
- <span data-ttu-id="11921-149">Postados</span><span class="sxs-lookup"><span data-stu-id="11921-149">Posted</span></span>
- <span data-ttu-id="11921-150">Ler</span><span class="sxs-lookup"><span data-stu-id="11921-150">Read</span></span>
- <span data-ttu-id="11921-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="11921-151">Report Date</span></span>
- <span data-ttu-id="11921-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="11921-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="11921-153">JSON</span><span class="sxs-lookup"><span data-stu-id="11921-153">JSON</span></span>

<span data-ttu-id="11921-154">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto yammerActivitySummary](../resources/yammeractivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11921-154">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11921-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11921-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="11921-156">CSV</span><span class="sxs-lookup"><span data-stu-id="11921-156">CSV</span></span>

<span data-ttu-id="11921-157">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="11921-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="11921-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11921-158">Request</span></span>

<span data-ttu-id="11921-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11921-159">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammeractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="11921-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="11921-160">Response</span></span>

<span data-ttu-id="11921-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11921-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="11921-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="11921-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="11921-163">JSON</span><span class="sxs-lookup"><span data-stu-id="11921-163">JSON</span></span>

<span data-ttu-id="11921-164">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="11921-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="11921-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11921-165">Request</span></span>

<span data-ttu-id="11921-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11921-166">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammeractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="11921-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="11921-167">Response</span></span>

<span data-ttu-id="11921-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11921-168">The following is an example of the response.</span></span>

> <span data-ttu-id="11921-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="11921-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 40, 
      "posted": 54, 
      "read": 28, 
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


