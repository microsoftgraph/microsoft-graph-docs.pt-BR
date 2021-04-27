---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Obtenha o número de usuários que usam dispositivos exclusivos em sua organização. O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 4a842a378aabf55171b3ca69b0a114793ced4577
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052828"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="628aa-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="628aa-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="628aa-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="628aa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="628aa-106">Obtenha o número de usuários que usam dispositivos exclusivos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="628aa-106">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="628aa-107">O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.</span><span class="sxs-lookup"><span data-stu-id="628aa-107">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="628aa-108">**Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Skype for Business clientes usados](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="628aa-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="628aa-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="628aa-109">Permissions</span></span>

<span data-ttu-id="628aa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="628aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="628aa-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="628aa-112">Permission type</span></span>                        | <span data-ttu-id="628aa-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="628aa-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="628aa-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="628aa-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="628aa-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="628aa-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="628aa-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="628aa-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="628aa-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="628aa-117">Not supported.</span></span>                           |
| <span data-ttu-id="628aa-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="628aa-118">Application</span></span>                            | <span data-ttu-id="628aa-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="628aa-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="628aa-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="628aa-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="628aa-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="628aa-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="628aa-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="628aa-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="628aa-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="628aa-123">Function parameters</span></span>

<span data-ttu-id="628aa-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="628aa-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="628aa-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="628aa-125">Parameter</span></span> | <span data-ttu-id="628aa-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="628aa-126">Type</span></span>   | <span data-ttu-id="628aa-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="628aa-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="628aa-128">ponto</span><span class="sxs-lookup"><span data-stu-id="628aa-128">period</span></span>    | <span data-ttu-id="628aa-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="628aa-129">string</span></span> | <span data-ttu-id="628aa-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="628aa-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="628aa-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="628aa-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="628aa-132">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="628aa-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="628aa-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="628aa-133">Required.</span></span> |

<span data-ttu-id="628aa-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="628aa-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="628aa-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="628aa-135">The default output type is text/csv.</span></span> <span data-ttu-id="628aa-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="628aa-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="628aa-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="628aa-137">Request headers</span></span>

| <span data-ttu-id="628aa-138">Nome</span><span class="sxs-lookup"><span data-stu-id="628aa-138">Name</span></span>          | <span data-ttu-id="628aa-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="628aa-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="628aa-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="628aa-140">Authorization</span></span> | <span data-ttu-id="628aa-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="628aa-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="628aa-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="628aa-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="628aa-144">CSV</span><span class="sxs-lookup"><span data-stu-id="628aa-144">CSV</span></span>

<span data-ttu-id="628aa-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="628aa-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="628aa-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="628aa-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="628aa-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="628aa-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="628aa-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="628aa-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="628aa-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="628aa-149">Report Refresh Date</span></span>
- <span data-ttu-id="628aa-150">Windows</span><span class="sxs-lookup"><span data-stu-id="628aa-150">Windows</span></span>
- <span data-ttu-id="628aa-151">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="628aa-151">Windows Phone</span></span>
- <span data-ttu-id="628aa-152">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="628aa-152">Android Phone</span></span>
- <span data-ttu-id="628aa-153">iPhone</span><span class="sxs-lookup"><span data-stu-id="628aa-153">iPhone</span></span>
- <span data-ttu-id="628aa-154">iPad</span><span class="sxs-lookup"><span data-stu-id="628aa-154">iPad</span></span>
- <span data-ttu-id="628aa-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="628aa-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="628aa-156">JSON</span><span class="sxs-lookup"><span data-stu-id="628aa-156">JSON</span></span>

<span data-ttu-id="628aa-157">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="628aa-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="628aa-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="628aa-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="628aa-159">CSV</span><span class="sxs-lookup"><span data-stu-id="628aa-159">CSV</span></span>

<span data-ttu-id="628aa-160">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="628aa-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="628aa-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="628aa-161">Request</span></span>

<span data-ttu-id="628aa-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="628aa-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="628aa-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="628aa-163">Response</span></span>

<span data-ttu-id="628aa-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="628aa-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="628aa-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="628aa-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="628aa-166">JSON</span><span class="sxs-lookup"><span data-stu-id="628aa-166">JSON</span></span>

<span data-ttu-id="628aa-167">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="628aa-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="628aa-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="628aa-168">Request</span></span>

<span data-ttu-id="628aa-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="628aa-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="628aa-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="628aa-170">Response</span></span>

<span data-ttu-id="628aa-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="628aa-171">The following is an example of the response.</span></span>

> <span data-ttu-id="628aa-172">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="628aa-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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


