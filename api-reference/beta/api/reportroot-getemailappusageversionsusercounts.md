---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook.
localization_priority: Normal
ms.openlocfilehash: 5ff2451ac4b3e50d7cd5ef2c6c31163c2e15235a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827907"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="bef89-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="bef89-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

> <span data-ttu-id="bef89-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bef89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bef89-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bef89-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bef89-106">Obtenha a contagem de usuários exclusivos por versão da área de trabalho do Outlook.</span><span class="sxs-lookup"><span data-stu-id="bef89-106">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="bef89-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="bef89-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="bef89-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bef89-108">Permissions</span></span>

<span data-ttu-id="bef89-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bef89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bef89-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bef89-111">Permission type</span></span>                        | <span data-ttu-id="bef89-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bef89-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bef89-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bef89-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bef89-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bef89-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bef89-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bef89-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bef89-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bef89-116">Not supported.</span></span>                           |
| <span data-ttu-id="bef89-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bef89-117">Application</span></span>                            | <span data-ttu-id="bef89-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bef89-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bef89-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bef89-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bef89-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="bef89-120">Function parameters</span></span>

<span data-ttu-id="bef89-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="bef89-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bef89-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bef89-122">Parameter</span></span> | <span data-ttu-id="bef89-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="bef89-123">Type</span></span>   | <span data-ttu-id="bef89-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bef89-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bef89-125">ponto</span><span class="sxs-lookup"><span data-stu-id="bef89-125">period</span></span>    | <span data-ttu-id="bef89-126">string</span><span class="sxs-lookup"><span data-stu-id="bef89-126">string</span></span> | <span data-ttu-id="bef89-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bef89-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bef89-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="bef89-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bef89-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bef89-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bef89-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bef89-130">Required.</span></span> |

<span data-ttu-id="bef89-131">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bef89-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bef89-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="bef89-132">The default output type is text/csv.</span></span> <span data-ttu-id="bef89-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="bef89-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bef89-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bef89-134">Request headers</span></span>

| <span data-ttu-id="bef89-135">Nome</span><span class="sxs-lookup"><span data-stu-id="bef89-135">Name</span></span>          | <span data-ttu-id="bef89-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="bef89-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bef89-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="bef89-137">Authorization</span></span> | <span data-ttu-id="bef89-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bef89-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bef89-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bef89-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bef89-141">CSV</span><span class="sxs-lookup"><span data-stu-id="bef89-141">CSV</span></span>

<span data-ttu-id="bef89-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="bef89-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bef89-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="bef89-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bef89-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bef89-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bef89-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="bef89-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bef89-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="bef89-146">Report Refresh Date</span></span>
- <span data-ttu-id="bef89-147">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="bef89-147">Outlook 2016</span></span>
- <span data-ttu-id="bef89-148">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="bef89-148">Outlook 2013</span></span>
- <span data-ttu-id="bef89-149">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="bef89-149">Outlook 2010</span></span>
- <span data-ttu-id="bef89-150">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="bef89-150">Outlook 2007</span></span>
- <span data-ttu-id="bef89-151">Indefinido</span><span class="sxs-lookup"><span data-stu-id="bef89-151">Undetermined</span></span>
- <span data-ttu-id="bef89-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="bef89-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bef89-153">JSON</span><span class="sxs-lookup"><span data-stu-id="bef89-153">JSON</span></span>

<span data-ttu-id="bef89-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bef89-154">If successful, this method returns a `200 OK` response code and an **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bef89-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bef89-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bef89-156">CSV</span><span class="sxs-lookup"><span data-stu-id="bef89-156">CSV</span></span>

<span data-ttu-id="bef89-157">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="bef89-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bef89-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bef89-158">Request</span></span>

<span data-ttu-id="bef89-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bef89-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="bef89-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="bef89-160">Response</span></span>

<span data-ttu-id="bef89-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bef89-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bef89-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="bef89-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
```

### <a name="json"></a><span data-ttu-id="bef89-163">JSON</span><span class="sxs-lookup"><span data-stu-id="bef89-163">JSON</span></span>

<span data-ttu-id="bef89-164">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="bef89-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bef89-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bef89-165">Request</span></span>

<span data-ttu-id="bef89-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bef89-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="bef89-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="bef89-167">Response</span></span>

<span data-ttu-id="bef89-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bef89-168">The following is an example of the response.</span></span>

> <span data-ttu-id="bef89-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bef89-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageVersionsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "outlook2016": 1554, 
      "outlook2013": 64, 
      "outlook2010": 1, 
      "outlook2007": 0, 
      "undetermined": 1259, 
      "reportPeriod": "7"
    }
  ]
}
```
