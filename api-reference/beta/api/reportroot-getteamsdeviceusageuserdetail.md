---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.
ms.openlocfilehash: 61954c3eb8853a74044d3da921985b63113c03b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039585"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="6c290-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="6c290-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

> <span data-ttu-id="6c290-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6c290-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c290-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6c290-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c290-106">Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="6c290-106">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c290-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c290-107">Permissions</span></span>

<span data-ttu-id="6c290-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c290-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c290-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c290-110">Permission type</span></span>                        | <span data-ttu-id="6c290-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c290-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6c290-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c290-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c290-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c290-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6c290-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c290-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c290-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c290-115">Not supported.</span></span>                           |
| <span data-ttu-id="6c290-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c290-116">Application</span></span>                            | <span data-ttu-id="6c290-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c290-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6c290-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c290-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="6c290-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="6c290-119">Function parameters</span></span>

<span data-ttu-id="6c290-120">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6c290-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="6c290-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6c290-121">Parameter</span></span> | <span data-ttu-id="6c290-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c290-122">Type</span></span>   | <span data-ttu-id="6c290-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c290-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6c290-124">ponto</span><span class="sxs-lookup"><span data-stu-id="6c290-124">period</span></span>    | <span data-ttu-id="6c290-125">string</span><span class="sxs-lookup"><span data-stu-id="6c290-125">string</span></span> | <span data-ttu-id="6c290-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6c290-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6c290-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="6c290-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6c290-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6c290-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="6c290-129">data</span><span class="sxs-lookup"><span data-stu-id="6c290-129">date</span></span>      | <span data-ttu-id="6c290-130">Data</span><span class="sxs-lookup"><span data-stu-id="6c290-130">Date</span></span>   | <span data-ttu-id="6c290-131">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="6c290-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="6c290-132">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="6c290-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="6c290-133">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="6c290-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="6c290-134">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="6c290-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="6c290-135">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="6c290-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6c290-136">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="6c290-136">The default output type is text/csv.</span></span> <span data-ttu-id="6c290-137">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="6c290-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c290-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c290-138">Request headers</span></span>

| <span data-ttu-id="6c290-139">Nome</span><span class="sxs-lookup"><span data-stu-id="6c290-139">Name</span></span>          | <span data-ttu-id="6c290-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c290-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6c290-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c290-141">Authorization</span></span> | <span data-ttu-id="6c290-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c290-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6c290-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c290-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6c290-145">CSV</span><span class="sxs-lookup"><span data-stu-id="6c290-145">CSV</span></span>

<span data-ttu-id="6c290-146">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="6c290-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6c290-147">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="6c290-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6c290-148">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6c290-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6c290-149">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="6c290-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6c290-150">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="6c290-150">Report Refresh Date</span></span>
- <span data-ttu-id="6c290-151">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="6c290-151">User Principal Name</span></span>
- <span data-ttu-id="6c290-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="6c290-152">Last Activity Date</span></span>
- <span data-ttu-id="6c290-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="6c290-153">Is Deleted</span></span>
- <span data-ttu-id="6c290-154">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="6c290-154">Deleted Date</span></span>
- <span data-ttu-id="6c290-155">Usou Web</span><span class="sxs-lookup"><span data-stu-id="6c290-155">Used Web</span></span>
- <span data-ttu-id="6c290-156">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="6c290-156">Used Windows Phone</span></span>
- <span data-ttu-id="6c290-157">Usou iOS</span><span class="sxs-lookup"><span data-stu-id="6c290-157">Used iOS</span></span>
- <span data-ttu-id="6c290-158">Usou Mac</span><span class="sxs-lookup"><span data-stu-id="6c290-158">Used Mac</span></span>
- <span data-ttu-id="6c290-159">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="6c290-159">Used Android Phone</span></span>
- <span data-ttu-id="6c290-160">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="6c290-160">Used Windows</span></span>
- <span data-ttu-id="6c290-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="6c290-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="6c290-162">JSON</span><span class="sxs-lookup"><span data-stu-id="6c290-162">JSON</span></span>

<span data-ttu-id="6c290-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c290-163">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="6c290-164">O tamanho de página padrão para essa solicitação é 2000 itens.</span><span class="sxs-lookup"><span data-stu-id="6c290-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="6c290-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c290-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6c290-166">CSV</span><span class="sxs-lookup"><span data-stu-id="6c290-166">CSV</span></span>

<span data-ttu-id="6c290-167">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="6c290-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6c290-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c290-168">Request</span></span>

<span data-ttu-id="6c290-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c290-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6c290-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c290-170">Response</span></span>

<span data-ttu-id="6c290-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6c290-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6c290-172">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="6c290-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="6c290-173">JSON</span><span class="sxs-lookup"><span data-stu-id="6c290-173">JSON</span></span>

<span data-ttu-id="6c290-174">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="6c290-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6c290-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c290-175">Request</span></span>

<span data-ttu-id="6c290-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c290-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6c290-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c290-177">Response</span></span>

<span data-ttu-id="6c290-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6c290-178">The following is an example of the response.</span></span>

> <span data-ttu-id="6c290-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c290-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
      "reportPeriod": "7"
    }
  ]
}
```
