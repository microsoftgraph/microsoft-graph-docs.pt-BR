---
title: 'reportRoot: getSharePointActivityFileCounts'
description: Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: e472684cbfdc250aa2d197cf06408bf10d09845e
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983629"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="e6605-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="e6605-103">reportRoot: getSharePointActivityFileCounts</span></span>

<span data-ttu-id="e6605-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6605-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6605-105">Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e6605-105">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="e6605-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte [relatórios do Microsoft 365 - atividade do SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)</span><span class="sxs-lookup"><span data-stu-id="e6605-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6605-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6605-107">Permissions</span></span>

<span data-ttu-id="e6605-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6605-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6605-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6605-110">Permission type</span></span>                        | <span data-ttu-id="e6605-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6605-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e6605-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6605-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6605-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6605-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e6605-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6605-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6605-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6605-115">Not supported.</span></span>                           |
| <span data-ttu-id="e6605-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6605-116">Application</span></span>                            | <span data-ttu-id="e6605-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6605-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="e6605-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="e6605-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e6605-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="e6605-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e6605-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6605-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e6605-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e6605-121">Function parameters</span></span>

<span data-ttu-id="e6605-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e6605-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e6605-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e6605-123">Parameter</span></span> | <span data-ttu-id="e6605-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6605-124">Type</span></span>   | <span data-ttu-id="e6605-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6605-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e6605-126">ponto</span><span class="sxs-lookup"><span data-stu-id="e6605-126">period</span></span>    | <span data-ttu-id="e6605-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6605-127">string</span></span> | <span data-ttu-id="e6605-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e6605-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e6605-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e6605-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e6605-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e6605-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e6605-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6605-131">Required.</span></span> |

<span data-ttu-id="e6605-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e6605-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e6605-133">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="e6605-133">The default output type is text/csv.</span></span> <span data-ttu-id="e6605-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="e6605-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6605-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6605-135">Request headers</span></span>

| <span data-ttu-id="e6605-136">Nome</span><span class="sxs-lookup"><span data-stu-id="e6605-136">Name</span></span>          | <span data-ttu-id="e6605-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6605-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e6605-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6605-138">Authorization</span></span> | <span data-ttu-id="e6605-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6605-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e6605-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6605-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e6605-142">CSV</span><span class="sxs-lookup"><span data-stu-id="e6605-142">CSV</span></span>

<span data-ttu-id="e6605-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e6605-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e6605-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e6605-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e6605-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e6605-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e6605-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e6605-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e6605-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e6605-147">Report Refresh Date</span></span>
- <span data-ttu-id="e6605-148">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="e6605-148">Viewed Or Edited</span></span>
- <span data-ttu-id="e6605-149">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="e6605-149">Synced</span></span>
- <span data-ttu-id="e6605-150">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="e6605-150">Shared Internally</span></span>
- <span data-ttu-id="e6605-151">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="e6605-151">Shared Externally</span></span>
- <span data-ttu-id="e6605-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="e6605-152">Report Date</span></span>
- <span data-ttu-id="e6605-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e6605-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e6605-154">JSON</span><span class="sxs-lookup"><span data-stu-id="e6605-154">JSON</span></span>

<span data-ttu-id="e6605-155">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` **[objeto siteActivitySummary](../resources/siteactivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6605-155">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6605-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6605-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e6605-157">CSV</span><span class="sxs-lookup"><span data-stu-id="e6605-157">CSV</span></span>

<span data-ttu-id="e6605-158">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="e6605-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e6605-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6605-159">Request</span></span>

<span data-ttu-id="e6605-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6605-160">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityfilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityFileCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="e6605-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6605-161">Response</span></span>

<span data-ttu-id="e6605-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6605-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e6605-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e6605-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="e6605-164">JSON</span><span class="sxs-lookup"><span data-stu-id="e6605-164">JSON</span></span>

<span data-ttu-id="e6605-165">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="e6605-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e6605-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6605-166">Request</span></span>

<span data-ttu-id="e6605-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6605-167">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="e6605-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6605-168">Response</span></span>

<span data-ttu-id="e6605-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6605-169">The following is an example of the response.</span></span>

> <span data-ttu-id="e6605-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6605-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 2141, 
      "synced": 614, 
      "sharedInternally": 9, 
      "sharedExternally": 0, 
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


