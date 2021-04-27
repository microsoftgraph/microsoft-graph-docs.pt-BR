---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business. Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 8b26281cf096f822718aea7268a75f69d1a1a9ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052821"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="745c2-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="745c2-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="745c2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="745c2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="745c2-106">Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="745c2-106">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="745c2-107">Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.</span><span class="sxs-lookup"><span data-stu-id="745c2-107">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="745c2-108">**Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Skype for Business clientes usados](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="745c2-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="745c2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="745c2-109">Permissions</span></span>

<span data-ttu-id="745c2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="745c2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="745c2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="745c2-112">Permission type</span></span>                        | <span data-ttu-id="745c2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="745c2-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="745c2-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="745c2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="745c2-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="745c2-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="745c2-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="745c2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="745c2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="745c2-117">Not supported.</span></span>                           |
| <span data-ttu-id="745c2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="745c2-118">Application</span></span>                            | <span data-ttu-id="745c2-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="745c2-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="745c2-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="745c2-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="745c2-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="745c2-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="745c2-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="745c2-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="745c2-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="745c2-123">Function parameters</span></span>

<span data-ttu-id="745c2-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="745c2-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="745c2-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="745c2-125">Parameter</span></span> | <span data-ttu-id="745c2-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="745c2-126">Type</span></span>   | <span data-ttu-id="745c2-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="745c2-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="745c2-128">ponto</span><span class="sxs-lookup"><span data-stu-id="745c2-128">period</span></span>    | <span data-ttu-id="745c2-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="745c2-129">string</span></span> | <span data-ttu-id="745c2-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="745c2-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="745c2-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="745c2-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="745c2-132">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="745c2-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="745c2-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="745c2-133">Required.</span></span> |

<span data-ttu-id="745c2-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="745c2-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="745c2-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="745c2-135">The default output type is text/csv.</span></span> <span data-ttu-id="745c2-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="745c2-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="745c2-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="745c2-137">Request headers</span></span>

| <span data-ttu-id="745c2-138">Nome</span><span class="sxs-lookup"><span data-stu-id="745c2-138">Name</span></span>          | <span data-ttu-id="745c2-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="745c2-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="745c2-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="745c2-140">Authorization</span></span> | <span data-ttu-id="745c2-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="745c2-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="745c2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="745c2-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="745c2-144">CSV</span><span class="sxs-lookup"><span data-stu-id="745c2-144">CSV</span></span>

<span data-ttu-id="745c2-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="745c2-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="745c2-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="745c2-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="745c2-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="745c2-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="745c2-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="745c2-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="745c2-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="745c2-149">Report Refresh Date</span></span>
- <span data-ttu-id="745c2-150">Windows</span><span class="sxs-lookup"><span data-stu-id="745c2-150">Windows</span></span>
- <span data-ttu-id="745c2-151">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="745c2-151">Windows Phone</span></span>
- <span data-ttu-id="745c2-152">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="745c2-152">Android Phone</span></span>
- <span data-ttu-id="745c2-153">iPhone</span><span class="sxs-lookup"><span data-stu-id="745c2-153">iPhone</span></span>
- <span data-ttu-id="745c2-154">iPad</span><span class="sxs-lookup"><span data-stu-id="745c2-154">iPad</span></span>
- <span data-ttu-id="745c2-155">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="745c2-155">Report Date</span></span>
- <span data-ttu-id="745c2-156">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="745c2-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="745c2-157">JSON</span><span class="sxs-lookup"><span data-stu-id="745c2-157">JSON</span></span>

<span data-ttu-id="745c2-158">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="745c2-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="745c2-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="745c2-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="745c2-160">CSV</span><span class="sxs-lookup"><span data-stu-id="745c2-160">CSV</span></span>

<span data-ttu-id="745c2-161">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="745c2-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="745c2-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="745c2-162">Request</span></span>

<span data-ttu-id="745c2-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="745c2-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="745c2-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="745c2-164">Response</span></span>

<span data-ttu-id="745c2-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="745c2-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="745c2-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="745c2-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="745c2-167">JSON</span><span class="sxs-lookup"><span data-stu-id="745c2-167">JSON</span></span>

<span data-ttu-id="745c2-168">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="745c2-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="745c2-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="745c2-169">Request</span></span>

<span data-ttu-id="745c2-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="745c2-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="745c2-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="745c2-171">Response</span></span>

<span data-ttu-id="745c2-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="745c2-172">The following is an example of the response.</span></span>

> <span data-ttu-id="745c2-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="745c2-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 403, 
      "windowsPhone": 2, 
      "androidPhone": 13, 
      "iPhone": 26, 
      "iPad": 0, 
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


