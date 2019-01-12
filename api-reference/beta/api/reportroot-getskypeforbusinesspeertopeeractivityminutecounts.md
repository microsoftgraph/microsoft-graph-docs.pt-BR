---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização. Tipos de sessões incluem áudio e vídeo.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 357c3d2e972cc70be4d517556946a6c08d56b447
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945080"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="2b846-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="2b846-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

> <span data-ttu-id="2b846-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2b846-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b846-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2b846-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b846-107">Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="2b846-107">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="2b846-108">Tipos de sessões incluem áudio e vídeo.</span><span class="sxs-lookup"><span data-stu-id="2b846-108">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="2b846-109">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="2b846-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b846-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b846-110">Permissions</span></span>

<span data-ttu-id="2b846-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b846-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b846-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b846-113">Permission type</span></span>                        | <span data-ttu-id="2b846-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b846-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2b846-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b846-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b846-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b846-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2b846-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b846-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b846-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b846-118">Not supported.</span></span>                           |
| <span data-ttu-id="2b846-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b846-119">Application</span></span>                            | <span data-ttu-id="2b846-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b846-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2b846-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b846-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2b846-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="2b846-122">Function parameters</span></span>

<span data-ttu-id="2b846-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="2b846-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2b846-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2b846-124">Parameter</span></span> | <span data-ttu-id="2b846-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b846-125">Type</span></span>   | <span data-ttu-id="2b846-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b846-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2b846-127">ponto</span><span class="sxs-lookup"><span data-stu-id="2b846-127">period</span></span>    | <span data-ttu-id="2b846-128">string</span><span class="sxs-lookup"><span data-stu-id="2b846-128">string</span></span> | <span data-ttu-id="2b846-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2b846-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2b846-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="2b846-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2b846-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="2b846-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2b846-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b846-132">Required.</span></span> |

<span data-ttu-id="2b846-133">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b846-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2b846-134">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="2b846-134">The default output type is text/csv.</span></span> <span data-ttu-id="2b846-135">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="2b846-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b846-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b846-136">Request headers</span></span>

| <span data-ttu-id="2b846-137">Nome</span><span class="sxs-lookup"><span data-stu-id="2b846-137">Name</span></span>          | <span data-ttu-id="2b846-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b846-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2b846-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b846-139">Authorization</span></span> | <span data-ttu-id="2b846-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b846-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2b846-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b846-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2b846-143">CSV</span><span class="sxs-lookup"><span data-stu-id="2b846-143">CSV</span></span>

<span data-ttu-id="2b846-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="2b846-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2b846-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="2b846-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2b846-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2b846-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2b846-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="2b846-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2b846-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="2b846-148">Report Refresh Date</span></span>
- <span data-ttu-id="2b846-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="2b846-149">Report Date</span></span>
- <span data-ttu-id="2b846-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="2b846-150">Report Period</span></span>
- <span data-ttu-id="2b846-151">Áudio</span><span class="sxs-lookup"><span data-stu-id="2b846-151">Audio</span></span>
- <span data-ttu-id="2b846-152">Vídeo</span><span class="sxs-lookup"><span data-stu-id="2b846-152">Video</span></span>

### <a name="json"></a><span data-ttu-id="2b846-153">JSON</span><span class="sxs-lookup"><span data-stu-id="2b846-153">JSON</span></span>

<span data-ttu-id="2b846-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b846-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b846-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b846-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2b846-156">CSV</span><span class="sxs-lookup"><span data-stu-id="2b846-156">CSV</span></span>

<span data-ttu-id="2b846-157">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="2b846-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2b846-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b846-158">Request</span></span>

<span data-ttu-id="2b846-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b846-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="2b846-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b846-160">Response</span></span>

<span data-ttu-id="2b846-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2b846-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2b846-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="2b846-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
```

### <a name="json"></a><span data-ttu-id="2b846-163">JSON</span><span class="sxs-lookup"><span data-stu-id="2b846-163">JSON</span></span>

<span data-ttu-id="2b846-164">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="2b846-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2b846-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b846-165">Request</span></span>

<span data-ttu-id="2b846-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b846-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="2b846-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b846-167">Response</span></span>

<span data-ttu-id="2b846-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2b846-168">The following is an example of the response.</span></span>

> <span data-ttu-id="2b846-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b846-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts)", 
  "value": [
    {
      "audio": 836, 
      "video": 35, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
