---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Obtenha o número de usuários que usam dispositivos exclusivos em sua organização. O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.
localization_priority: Normal
ms.openlocfilehash: 87385d36b6af3451b71a7886c9da7187b4a2c1ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831798"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="a80ed-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="a80ed-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="a80ed-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a80ed-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a80ed-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a80ed-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a80ed-107">Obtenha o número de usuários que usam dispositivos exclusivos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="a80ed-107">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="a80ed-108">O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.</span><span class="sxs-lookup"><span data-stu-id="a80ed-108">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="a80ed-109">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="a80ed-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="a80ed-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a80ed-110">Permissions</span></span>

<span data-ttu-id="a80ed-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a80ed-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a80ed-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a80ed-113">Permission type</span></span>                        | <span data-ttu-id="a80ed-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a80ed-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a80ed-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a80ed-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="a80ed-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a80ed-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a80ed-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a80ed-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a80ed-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a80ed-118">Not supported.</span></span>                           |
| <span data-ttu-id="a80ed-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a80ed-119">Application</span></span>                            | <span data-ttu-id="a80ed-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a80ed-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a80ed-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a80ed-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a80ed-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a80ed-122">Function parameters</span></span>

<span data-ttu-id="a80ed-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a80ed-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a80ed-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a80ed-124">Parameter</span></span> | <span data-ttu-id="a80ed-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="a80ed-125">Type</span></span>   | <span data-ttu-id="a80ed-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="a80ed-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a80ed-127">ponto</span><span class="sxs-lookup"><span data-stu-id="a80ed-127">period</span></span>    | <span data-ttu-id="a80ed-128">string</span><span class="sxs-lookup"><span data-stu-id="a80ed-128">string</span></span> | <span data-ttu-id="a80ed-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a80ed-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a80ed-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a80ed-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a80ed-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a80ed-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a80ed-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a80ed-132">Required.</span></span> |

<span data-ttu-id="a80ed-133">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a80ed-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a80ed-134">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="a80ed-134">The default output type is text/csv.</span></span> <span data-ttu-id="a80ed-135">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="a80ed-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a80ed-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a80ed-136">Request headers</span></span>

| <span data-ttu-id="a80ed-137">Nome</span><span class="sxs-lookup"><span data-stu-id="a80ed-137">Name</span></span>          | <span data-ttu-id="a80ed-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="a80ed-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a80ed-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="a80ed-139">Authorization</span></span> | <span data-ttu-id="a80ed-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a80ed-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a80ed-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a80ed-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a80ed-143">CSV</span><span class="sxs-lookup"><span data-stu-id="a80ed-143">CSV</span></span>

<span data-ttu-id="a80ed-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a80ed-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a80ed-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a80ed-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a80ed-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a80ed-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a80ed-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a80ed-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a80ed-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a80ed-148">Report Refresh Date</span></span>
- <span data-ttu-id="a80ed-149">Windows</span><span class="sxs-lookup"><span data-stu-id="a80ed-149">Windows</span></span>
- <span data-ttu-id="a80ed-150">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="a80ed-150">Windows Phone</span></span>
- <span data-ttu-id="a80ed-151">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="a80ed-151">Android Phone</span></span>
- <span data-ttu-id="a80ed-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="a80ed-152">iPhone</span></span>
- <span data-ttu-id="a80ed-153">iPad</span><span class="sxs-lookup"><span data-stu-id="a80ed-153">iPad</span></span>
- <span data-ttu-id="a80ed-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a80ed-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a80ed-155">JSON</span><span class="sxs-lookup"><span data-stu-id="a80ed-155">JSON</span></span>

<span data-ttu-id="a80ed-156">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a80ed-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a80ed-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a80ed-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a80ed-158">CSV</span><span class="sxs-lookup"><span data-stu-id="a80ed-158">CSV</span></span>

<span data-ttu-id="a80ed-159">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="a80ed-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a80ed-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a80ed-160">Request</span></span>

<span data-ttu-id="a80ed-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a80ed-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="a80ed-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="a80ed-162">Response</span></span>

<span data-ttu-id="a80ed-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a80ed-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a80ed-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a80ed-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a80ed-165">JSON</span><span class="sxs-lookup"><span data-stu-id="a80ed-165">JSON</span></span>

<span data-ttu-id="a80ed-166">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="a80ed-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a80ed-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a80ed-167">Request</span></span>

<span data-ttu-id="a80ed-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a80ed-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="a80ed-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="a80ed-169">Response</span></span>

<span data-ttu-id="a80ed-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a80ed-170">The following is an example of the response.</span></span>

> <span data-ttu-id="a80ed-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a80ed-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
