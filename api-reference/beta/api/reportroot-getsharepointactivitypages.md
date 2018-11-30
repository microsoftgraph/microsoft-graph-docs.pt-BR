---
title: 'reportRoot: getSharePointActivityPages'
description: Obtenha o número de páginas exclusivas visitadas pelos usuários.
ms.openlocfilehash: b9e98eebccb82061d4a601068d4e953fb3f246b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034144"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="17a38-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="17a38-103">reportRoot: getSharePointActivityPages</span></span>

> <span data-ttu-id="17a38-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="17a38-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17a38-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17a38-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17a38-106">Obtenha o número de páginas exclusivas visitadas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="17a38-106">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="17a38-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="17a38-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="17a38-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="17a38-108">Permissions</span></span>

<span data-ttu-id="17a38-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17a38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="17a38-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17a38-111">Permission type</span></span>                        | <span data-ttu-id="17a38-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17a38-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="17a38-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17a38-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="17a38-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="17a38-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="17a38-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17a38-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17a38-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17a38-116">Not supported.</span></span>                           |
| <span data-ttu-id="17a38-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17a38-117">Application</span></span>                            | <span data-ttu-id="17a38-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="17a38-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="17a38-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17a38-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="17a38-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="17a38-120">Function parameters</span></span>

<span data-ttu-id="17a38-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="17a38-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="17a38-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="17a38-122">Parameter</span></span> | <span data-ttu-id="17a38-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="17a38-123">Type</span></span>   | <span data-ttu-id="17a38-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="17a38-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="17a38-125">ponto</span><span class="sxs-lookup"><span data-stu-id="17a38-125">period</span></span>    | <span data-ttu-id="17a38-126">string</span><span class="sxs-lookup"><span data-stu-id="17a38-126">string</span></span> | <span data-ttu-id="17a38-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="17a38-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="17a38-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="17a38-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="17a38-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="17a38-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="17a38-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17a38-130">Required.</span></span> |

<span data-ttu-id="17a38-131">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="17a38-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="17a38-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="17a38-132">The default output type is text/csv.</span></span> <span data-ttu-id="17a38-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="17a38-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17a38-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17a38-134">Request headers</span></span>

| <span data-ttu-id="17a38-135">Nome</span><span class="sxs-lookup"><span data-stu-id="17a38-135">Name</span></span>          | <span data-ttu-id="17a38-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="17a38-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="17a38-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="17a38-137">Authorization</span></span> | <span data-ttu-id="17a38-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17a38-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="17a38-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="17a38-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="17a38-141">CSV</span><span class="sxs-lookup"><span data-stu-id="17a38-141">CSV</span></span>

<span data-ttu-id="17a38-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="17a38-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="17a38-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="17a38-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="17a38-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="17a38-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="17a38-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="17a38-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="17a38-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="17a38-146">Report Refresh Date</span></span>
- <span data-ttu-id="17a38-147">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="17a38-147">Visited Page Count</span></span>
- <span data-ttu-id="17a38-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="17a38-148">Report Date</span></span>
- <span data-ttu-id="17a38-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="17a38-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="17a38-150">JSON</span><span class="sxs-lookup"><span data-stu-id="17a38-150">JSON</span></span>

<span data-ttu-id="17a38-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[sharePointActivityPages](../resources/sharepointactivitypages.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17a38-151">If successful, this method returns a `200 OK` response code and a **[sharePointActivityPages](../resources/sharepointactivitypages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17a38-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17a38-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="17a38-153">CSV</span><span class="sxs-lookup"><span data-stu-id="17a38-153">CSV</span></span>

<span data-ttu-id="17a38-154">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="17a38-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="17a38-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17a38-155">Request</span></span>

<span data-ttu-id="17a38-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="17a38-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="17a38-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="17a38-157">Response</span></span>

<span data-ttu-id="17a38-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="17a38-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="17a38-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="17a38-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="17a38-160">JSON</span><span class="sxs-lookup"><span data-stu-id="17a38-160">JSON</span></span>

<span data-ttu-id="17a38-161">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="17a38-161">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="17a38-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17a38-162">Request</span></span>

<span data-ttu-id="17a38-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="17a38-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="17a38-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="17a38-164">Response</span></span>

<span data-ttu-id="17a38-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="17a38-165">The following is an example of the response.</span></span>

> <span data-ttu-id="17a38-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17a38-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
