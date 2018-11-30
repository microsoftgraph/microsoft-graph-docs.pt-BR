---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Obtenha o número de usuários que usam dispositivos exclusivos em sua organização. O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.
ms.openlocfilehash: bee105fc41d18543c611f05d2a3e389ff6a84526
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035080"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="7c8fc-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="7c8fc-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="7c8fc-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c8fc-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c8fc-107">Obtenha o número de usuários que usam dispositivos exclusivos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-107">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="7c8fc-108">O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-108">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="7c8fc-109">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="7c8fc-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c8fc-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c8fc-110">Permissions</span></span>

<span data-ttu-id="7c8fc-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c8fc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c8fc-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c8fc-113">Permission type</span></span>                        | <span data-ttu-id="7c8fc-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c8fc-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7c8fc-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c8fc-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c8fc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c8fc-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7c8fc-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c8fc-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c8fc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-118">Not supported.</span></span>                           |
| <span data-ttu-id="7c8fc-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c8fc-119">Application</span></span>                            | <span data-ttu-id="7c8fc-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c8fc-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7c8fc-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c8fc-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7c8fc-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7c8fc-122">Function parameters</span></span>

<span data-ttu-id="7c8fc-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7c8fc-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7c8fc-124">Parameter</span></span> | <span data-ttu-id="7c8fc-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c8fc-125">Type</span></span>   | <span data-ttu-id="7c8fc-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c8fc-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7c8fc-127">ponto</span><span class="sxs-lookup"><span data-stu-id="7c8fc-127">period</span></span>    | <span data-ttu-id="7c8fc-128">string</span><span class="sxs-lookup"><span data-stu-id="7c8fc-128">string</span></span> | <span data-ttu-id="7c8fc-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7c8fc-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7c8fc-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7c8fc-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-132">Required.</span></span> |

<span data-ttu-id="7c8fc-133">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7c8fc-134">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-134">The default output type is text/csv.</span></span> <span data-ttu-id="7c8fc-135">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c8fc-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8fc-136">Request headers</span></span>

| <span data-ttu-id="7c8fc-137">Nome</span><span class="sxs-lookup"><span data-stu-id="7c8fc-137">Name</span></span>          | <span data-ttu-id="7c8fc-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c8fc-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7c8fc-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c8fc-139">Authorization</span></span> | <span data-ttu-id="7c8fc-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7c8fc-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c8fc-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7c8fc-143">CSV</span><span class="sxs-lookup"><span data-stu-id="7c8fc-143">CSV</span></span>

<span data-ttu-id="7c8fc-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7c8fc-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7c8fc-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7c8fc-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7c8fc-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7c8fc-148">Report Refresh Date</span></span>
- <span data-ttu-id="7c8fc-149">Windows</span><span class="sxs-lookup"><span data-stu-id="7c8fc-149">Windows</span></span>
- <span data-ttu-id="7c8fc-150">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="7c8fc-150">Windows Phone</span></span>
- <span data-ttu-id="7c8fc-151">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="7c8fc-151">Android Phone</span></span>
- <span data-ttu-id="7c8fc-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="7c8fc-152">iPhone</span></span>
- <span data-ttu-id="7c8fc-153">iPad</span><span class="sxs-lookup"><span data-stu-id="7c8fc-153">iPad</span></span>
- <span data-ttu-id="7c8fc-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7c8fc-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7c8fc-155">JSON</span><span class="sxs-lookup"><span data-stu-id="7c8fc-155">JSON</span></span>

<span data-ttu-id="7c8fc-156">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c8fc-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c8fc-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7c8fc-158">CSV</span><span class="sxs-lookup"><span data-stu-id="7c8fc-158">CSV</span></span>

<span data-ttu-id="7c8fc-159">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7c8fc-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8fc-160">Request</span></span>

<span data-ttu-id="7c8fc-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="7c8fc-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c8fc-162">Response</span></span>

<span data-ttu-id="7c8fc-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7c8fc-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="7c8fc-165">JSON</span><span class="sxs-lookup"><span data-stu-id="7c8fc-165">JSON</span></span>

<span data-ttu-id="7c8fc-166">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7c8fc-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c8fc-167">Request</span></span>

<span data-ttu-id="7c8fc-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="7c8fc-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c8fc-169">Response</span></span>

<span data-ttu-id="7c8fc-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-170">The following is an example of the response.</span></span>

> <span data-ttu-id="7c8fc-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 122, 
      "windowsPhone": 8, 
      "androidPhone": 19, 
      "iPhone": 28, 
      "iPad": 1, 
      "reportPeriod": "7"
    }
  ]
}
```
