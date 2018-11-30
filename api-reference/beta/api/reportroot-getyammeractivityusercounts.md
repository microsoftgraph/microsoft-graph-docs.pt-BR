---
title: 'reportRoot: getYammerActivityUserCounts'
description: Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.
ms.openlocfilehash: 6df8a0f16e8cb4c10e05484eeecf1f4e60c4c889
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041212"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="46e57-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="46e57-103">reportRoot: getYammerActivityUserCounts</span></span>

> <span data-ttu-id="46e57-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="46e57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46e57-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46e57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46e57-106">Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer.</span><span class="sxs-lookup"><span data-stu-id="46e57-106">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="46e57-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="46e57-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="46e57-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="46e57-108">Permissions</span></span>

<span data-ttu-id="46e57-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46e57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46e57-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46e57-111">Permission type</span></span>                        | <span data-ttu-id="46e57-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46e57-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="46e57-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46e57-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="46e57-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="46e57-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="46e57-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46e57-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46e57-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46e57-116">Not supported.</span></span>                           |
| <span data-ttu-id="46e57-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46e57-117">Application</span></span>                            | <span data-ttu-id="46e57-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="46e57-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="46e57-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46e57-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="46e57-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="46e57-120">Function parameters</span></span>

<span data-ttu-id="46e57-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="46e57-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="46e57-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="46e57-122">Parameter</span></span> | <span data-ttu-id="46e57-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="46e57-123">Type</span></span>   | <span data-ttu-id="46e57-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="46e57-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="46e57-125">ponto</span><span class="sxs-lookup"><span data-stu-id="46e57-125">period</span></span>    | <span data-ttu-id="46e57-126">string</span><span class="sxs-lookup"><span data-stu-id="46e57-126">string</span></span> | <span data-ttu-id="46e57-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="46e57-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="46e57-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="46e57-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="46e57-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="46e57-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="46e57-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46e57-130">Required.</span></span> |

<span data-ttu-id="46e57-131">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="46e57-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="46e57-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="46e57-132">The default output type is text/csv.</span></span> <span data-ttu-id="46e57-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="46e57-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46e57-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46e57-134">Request headers</span></span>

| <span data-ttu-id="46e57-135">Nome</span><span class="sxs-lookup"><span data-stu-id="46e57-135">Name</span></span>          | <span data-ttu-id="46e57-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="46e57-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="46e57-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="46e57-137">Authorization</span></span> | <span data-ttu-id="46e57-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46e57-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="46e57-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="46e57-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="46e57-141">CSV</span><span class="sxs-lookup"><span data-stu-id="46e57-141">CSV</span></span>

<span data-ttu-id="46e57-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="46e57-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="46e57-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="46e57-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="46e57-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="46e57-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="46e57-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="46e57-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="46e57-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="46e57-146">Report Refresh Date</span></span>
- <span data-ttu-id="46e57-147">Curtidos</span><span class="sxs-lookup"><span data-stu-id="46e57-147">Liked</span></span>
- <span data-ttu-id="46e57-148">Postados</span><span class="sxs-lookup"><span data-stu-id="46e57-148">Posted</span></span>
- <span data-ttu-id="46e57-149">Ler</span><span class="sxs-lookup"><span data-stu-id="46e57-149">Read</span></span>
- <span data-ttu-id="46e57-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="46e57-150">Report Date</span></span>
- <span data-ttu-id="46e57-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="46e57-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="46e57-152">JSON</span><span class="sxs-lookup"><span data-stu-id="46e57-152">JSON</span></span>

<span data-ttu-id="46e57-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[yammerActivitySummary](../resources/yammeractivitysummary.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46e57-153">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46e57-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46e57-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="46e57-155">CSV</span><span class="sxs-lookup"><span data-stu-id="46e57-155">CSV</span></span>

<span data-ttu-id="46e57-156">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="46e57-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="46e57-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46e57-157">Request</span></span>

<span data-ttu-id="46e57-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46e57-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="46e57-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="46e57-159">Response</span></span>

<span data-ttu-id="46e57-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46e57-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="46e57-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="46e57-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="46e57-162">JSON</span><span class="sxs-lookup"><span data-stu-id="46e57-162">JSON</span></span>

<span data-ttu-id="46e57-163">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="46e57-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="46e57-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46e57-164">Request</span></span>

<span data-ttu-id="46e57-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46e57-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="46e57-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="46e57-166">Response</span></span>

<span data-ttu-id="46e57-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46e57-167">The following is an example of the response.</span></span>

> <span data-ttu-id="46e57-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46e57-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
