---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Obtenha a contagem de usuários por tipo de atividade e serviço.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 1911b570d046f192d57435d58c7473333aa53e60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956168"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="b7f74-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="b7f74-103">reportRoot: getOffice365ServicesUserCounts</span></span>

> <span data-ttu-id="b7f74-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b7f74-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7f74-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b7f74-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7f74-106">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="b7f74-106">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="b7f74-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="b7f74-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7f74-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7f74-108">Permissions</span></span>

<span data-ttu-id="b7f74-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7f74-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7f74-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7f74-111">Permission type</span></span>                        | <span data-ttu-id="b7f74-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7f74-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b7f74-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7f74-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7f74-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7f74-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b7f74-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7f74-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7f74-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7f74-116">Not supported.</span></span>                           |
| <span data-ttu-id="b7f74-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-117">Application</span></span>                            | <span data-ttu-id="b7f74-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7f74-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b7f74-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7f74-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b7f74-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b7f74-120">Function parameters</span></span>

<span data-ttu-id="b7f74-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b7f74-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b7f74-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b7f74-122">Parameter</span></span> | <span data-ttu-id="b7f74-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7f74-123">Type</span></span>   | <span data-ttu-id="b7f74-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7f74-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b7f74-125">ponto</span><span class="sxs-lookup"><span data-stu-id="b7f74-125">period</span></span>    | <span data-ttu-id="b7f74-126">string</span><span class="sxs-lookup"><span data-stu-id="b7f74-126">string</span></span> | <span data-ttu-id="b7f74-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b7f74-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b7f74-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b7f74-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b7f74-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b7f74-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b7f74-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7f74-130">Required.</span></span> |

<span data-ttu-id="b7f74-131">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b7f74-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b7f74-132">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="b7f74-132">The default output type is text/csv.</span></span> <span data-ttu-id="b7f74-133">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="b7f74-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7f74-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f74-134">Request headers</span></span>

| <span data-ttu-id="b7f74-135">Nome</span><span class="sxs-lookup"><span data-stu-id="b7f74-135">Name</span></span>          | <span data-ttu-id="b7f74-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7f74-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b7f74-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7f74-137">Authorization</span></span> | <span data-ttu-id="b7f74-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7f74-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b7f74-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7f74-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b7f74-141">CSV</span><span class="sxs-lookup"><span data-stu-id="b7f74-141">CSV</span></span>

<span data-ttu-id="b7f74-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b7f74-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b7f74-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b7f74-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b7f74-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b7f74-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b7f74-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b7f74-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b7f74-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b7f74-146">Report Refresh Date</span></span>
- <span data-ttu-id="b7f74-147">Exchange ativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-147">Exchange Active</span></span>
- <span data-ttu-id="b7f74-148">Exchange inativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-148">Exchange Inactive</span></span>
- <span data-ttu-id="b7f74-149">OneDrive ativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-149">OneDrive Active</span></span>
- <span data-ttu-id="b7f74-150">OneDrive inativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-150">OneDrive Inactive</span></span>
- <span data-ttu-id="b7f74-151">SharePoint ativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-151">SharePoint Active</span></span>
- <span data-ttu-id="b7f74-152">SharePoint inativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-152">SharePoint Inactive</span></span>
- <span data-ttu-id="b7f74-153">Skype for Business ativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-153">Skype For Business Active</span></span>
- <span data-ttu-id="b7f74-154">Skype for Business inativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-154">Skype For Business Inactive</span></span>
- <span data-ttu-id="b7f74-155">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="b7f74-155">Yammer Active</span></span>
- <span data-ttu-id="b7f74-156">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="b7f74-156">Yammer Inactive</span></span>
- <span data-ttu-id="b7f74-157">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-157">Teams Active</span></span>
- <span data-ttu-id="b7f74-158">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-158">Teams Inactive</span></span>
- <span data-ttu-id="b7f74-159">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b7f74-159">Report Period</span></span>

<span data-ttu-id="b7f74-160">Não há suporte para as seguintes colunas na China Microsoft Graph operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="b7f74-160">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="b7f74-161">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="b7f74-161">Yammer Active</span></span>
- <span data-ttu-id="b7f74-162">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="b7f74-162">Yammer Inactive</span></span>
- <span data-ttu-id="b7f74-163">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-163">Teams Active</span></span>
- <span data-ttu-id="b7f74-164">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="b7f74-164">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="b7f74-165">JSON</span><span class="sxs-lookup"><span data-stu-id="b7f74-165">JSON</span></span>

<span data-ttu-id="b7f74-166">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7f74-166">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="b7f74-167">Não há suporte para as seguintes propriedades no objeto **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** na China Microsoft Graph operado pela 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="b7f74-167">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="b7f74-168">yammerActive</span><span class="sxs-lookup"><span data-stu-id="b7f74-168">yammerActive</span></span>
- <span data-ttu-id="b7f74-169">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="b7f74-169">yammerInactive</span></span>
- <span data-ttu-id="b7f74-170">teamsActive</span><span class="sxs-lookup"><span data-stu-id="b7f74-170">teamsActive</span></span>
- <span data-ttu-id="b7f74-171">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="b7f74-171">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="b7f74-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7f74-172">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b7f74-173">CSV</span><span class="sxs-lookup"><span data-stu-id="b7f74-173">CSV</span></span>

<span data-ttu-id="b7f74-174">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="b7f74-174">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b7f74-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f74-175">Request</span></span>

<span data-ttu-id="b7f74-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7f74-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b7f74-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7f74-177">Response</span></span>

<span data-ttu-id="b7f74-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b7f74-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b7f74-179">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b7f74-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```

### <a name="json"></a><span data-ttu-id="b7f74-180">JSON</span><span class="sxs-lookup"><span data-stu-id="b7f74-180">JSON</span></span> 

<span data-ttu-id="b7f74-181">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="b7f74-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b7f74-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7f74-182">Request</span></span>

<span data-ttu-id="b7f74-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7f74-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b7f74-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7f74-184">Response</span></span>

<span data-ttu-id="b7f74-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b7f74-185">The following is an example of the response.</span></span>

> <span data-ttu-id="b7f74-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7f74-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 458

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ServicesUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeActive": 2591, 
      "exchangeInactive": 1426, 
      "oneDriveActive": 1800, 
      "oneDriveInactive": 2451, 
      "sharePointActive": 2286, 
      "sharePointInactive": 1815, 
      "skypeForBusinessActive": 2463, 
      "skypeForBusinessInactive": 1947, 
      "yammerActive": 473, 
      "yammerInactive": 2526, 
      "teamsActive": 846, 
      "teamsInactive": 1960, 
      "reportPeriod": "7"
    }
  ]
}
```
