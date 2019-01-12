---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a48cd5ed0cb4d2874c73502beb3fe2da09d330c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964596"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="87603-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="87603-104">reportRoot: getSharePointActivityUserCounts</span></span>

> <span data-ttu-id="87603-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="87603-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87603-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87603-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87603-107">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="87603-107">Get the trend in the number of active users.</span></span> <span data-ttu-id="87603-108">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="87603-108">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="87603-109">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="87603-109">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="87603-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="87603-110">Permissions</span></span>

<span data-ttu-id="87603-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87603-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87603-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87603-113">Permission type</span></span>                        | <span data-ttu-id="87603-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87603-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="87603-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87603-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="87603-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="87603-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="87603-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87603-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87603-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87603-118">Not supported.</span></span>                           |
| <span data-ttu-id="87603-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87603-119">Application</span></span>                            | <span data-ttu-id="87603-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="87603-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="87603-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87603-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="87603-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="87603-122">Function parameters</span></span>

<span data-ttu-id="87603-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="87603-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="87603-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="87603-124">Parameter</span></span> | <span data-ttu-id="87603-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="87603-125">Type</span></span>   | <span data-ttu-id="87603-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="87603-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="87603-127">ponto</span><span class="sxs-lookup"><span data-stu-id="87603-127">period</span></span>    | <span data-ttu-id="87603-128">string</span><span class="sxs-lookup"><span data-stu-id="87603-128">string</span></span> | <span data-ttu-id="87603-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="87603-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="87603-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="87603-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="87603-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="87603-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="87603-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87603-132">Required.</span></span> |

<span data-ttu-id="87603-133">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87603-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="87603-134">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="87603-134">The default output type is text/csv.</span></span> <span data-ttu-id="87603-135">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="87603-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87603-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87603-136">Request headers</span></span>

| <span data-ttu-id="87603-137">Nome</span><span class="sxs-lookup"><span data-stu-id="87603-137">Name</span></span>          | <span data-ttu-id="87603-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="87603-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="87603-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="87603-139">Authorization</span></span> | <span data-ttu-id="87603-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87603-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="87603-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="87603-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="87603-143">CSV</span><span class="sxs-lookup"><span data-stu-id="87603-143">CSV</span></span>

<span data-ttu-id="87603-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="87603-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="87603-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="87603-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="87603-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="87603-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="87603-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="87603-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="87603-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="87603-148">Report Refresh Date</span></span>
- <span data-ttu-id="87603-149">Página visitada</span><span class="sxs-lookup"><span data-stu-id="87603-149">Visited Page</span></span>
- <span data-ttu-id="87603-150">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="87603-150">Viewed Or Edited</span></span>
- <span data-ttu-id="87603-151">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="87603-151">Synced</span></span>
- <span data-ttu-id="87603-152">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="87603-152">Shared Internally</span></span>
- <span data-ttu-id="87603-153">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="87603-153">Shared Externally</span></span>
- <span data-ttu-id="87603-154">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="87603-154">Report Date</span></span>
- <span data-ttu-id="87603-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="87603-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="87603-156">JSON</span><span class="sxs-lookup"><span data-stu-id="87603-156">JSON</span></span>

<span data-ttu-id="87603-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87603-157">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87603-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87603-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="87603-159">CSV</span><span class="sxs-lookup"><span data-stu-id="87603-159">CSV</span></span>

<span data-ttu-id="87603-160">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="87603-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="87603-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87603-161">Request</span></span>

<span data-ttu-id="87603-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87603-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="87603-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="87603-163">Response</span></span>

<span data-ttu-id="87603-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87603-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="87603-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="87603-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="87603-166">JSON</span><span class="sxs-lookup"><span data-stu-id="87603-166">JSON</span></span>

<span data-ttu-id="87603-167">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="87603-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="87603-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87603-168">Request</span></span>

<span data-ttu-id="87603-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87603-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="87603-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="87603-170">Response</span></span>

<span data-ttu-id="87603-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87603-171">The following is an example of the response.</span></span>

> <span data-ttu-id="87603-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87603-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
