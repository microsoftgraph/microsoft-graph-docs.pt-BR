---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Obtém o número de usuários exclusivos diários do Microsoft Teams por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: e04d0ca1a0c283aca593e0a17dadc24f564045f4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983220"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="5b625-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="5b625-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="5b625-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b625-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b625-105">Obtém o número de usuários exclusivos diários do Microsoft Teams por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5b625-105">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b625-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b625-106">Permissions</span></span>

<span data-ttu-id="5b625-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b625-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b625-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b625-109">Permission type</span></span>                        | <span data-ttu-id="5b625-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b625-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5b625-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b625-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b625-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b625-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5b625-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b625-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b625-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b625-114">Not supported.</span></span>                           |
| <span data-ttu-id="5b625-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b625-115">Application</span></span>                            | <span data-ttu-id="5b625-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b625-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="5b625-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="5b625-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5b625-118">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5b625-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5b625-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b625-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="5b625-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5b625-120">Function parameters</span></span>

<span data-ttu-id="5b625-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5b625-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5b625-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5b625-122">Parameter</span></span> | <span data-ttu-id="5b625-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b625-123">Type</span></span>   | <span data-ttu-id="5b625-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b625-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5b625-125">ponto</span><span class="sxs-lookup"><span data-stu-id="5b625-125">period</span></span>    | <span data-ttu-id="5b625-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b625-126">string</span></span> | <span data-ttu-id="5b625-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5b625-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5b625-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5b625-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5b625-129">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5b625-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5b625-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b625-130">Required.</span></span> |

<span data-ttu-id="5b625-131">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5b625-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5b625-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="5b625-132">The default output type is text/csv.</span></span> <span data-ttu-id="5b625-133">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="5b625-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b625-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b625-134">Request headers</span></span>

| <span data-ttu-id="5b625-135">Nome</span><span class="sxs-lookup"><span data-stu-id="5b625-135">Name</span></span>          | <span data-ttu-id="5b625-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b625-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5b625-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b625-137">Authorization</span></span> | <span data-ttu-id="5b625-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b625-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5b625-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b625-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5b625-141">CSV</span><span class="sxs-lookup"><span data-stu-id="5b625-141">CSV</span></span>

<span data-ttu-id="5b625-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5b625-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5b625-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5b625-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5b625-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5b625-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5b625-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5b625-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5b625-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5b625-146">Report Refresh Date</span></span>
- <span data-ttu-id="5b625-147">Web</span><span class="sxs-lookup"><span data-stu-id="5b625-147">Web</span></span>
- <span data-ttu-id="5b625-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="5b625-148">Windows Phone</span></span>
- <span data-ttu-id="5b625-149">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="5b625-149">Android Phone</span></span>
- <span data-ttu-id="5b625-150">iOS</span><span class="sxs-lookup"><span data-stu-id="5b625-150">iOS</span></span>
- <span data-ttu-id="5b625-151">Mac</span><span class="sxs-lookup"><span data-stu-id="5b625-151">Mac</span></span>
- <span data-ttu-id="5b625-152">Windows</span><span class="sxs-lookup"><span data-stu-id="5b625-152">Windows</span></span>
- <span data-ttu-id="5b625-153">Data do Relatório</span><span class="sxs-lookup"><span data-stu-id="5b625-153">Report Date</span></span>
- <span data-ttu-id="5b625-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5b625-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5b625-155">JSON</span><span class="sxs-lookup"><span data-stu-id="5b625-155">JSON</span></span>

<span data-ttu-id="5b625-156">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b625-156">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b625-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b625-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5b625-158">CSV</span><span class="sxs-lookup"><span data-stu-id="5b625-158">CSV</span></span>

<span data-ttu-id="5b625-159">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="5b625-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5b625-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b625-160">Request</span></span>

<span data-ttu-id="5b625-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b625-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="5b625-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b625-162">Response</span></span>

<span data-ttu-id="5b625-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5b625-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5b625-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5b625-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="5b625-165">JSON</span><span class="sxs-lookup"><span data-stu-id="5b625-165">JSON</span></span>

<span data-ttu-id="5b625-166">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="5b625-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5b625-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b625-167">Request</span></span>

<span data-ttu-id="5b625-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b625-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="5b625-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b625-169">Response</span></span>

<span data-ttu-id="5b625-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5b625-170">The following is an example of the response.</span></span>

> <span data-ttu-id="5b625-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b625-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 13, 
      "windowsPhone": 0, 
      "androidPhone": 22, 
      "ios": 75, 
      "mac": 16, 
      "windows": 257, 
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


