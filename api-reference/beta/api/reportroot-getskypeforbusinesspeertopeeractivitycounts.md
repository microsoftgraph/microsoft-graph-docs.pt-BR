---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos.
ms.openlocfilehash: b489db8827e951e734d0b0d292e3782f3c809c5a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034737"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="76084-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="76084-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

> <span data-ttu-id="76084-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="76084-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76084-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="76084-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76084-107">Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="76084-107">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="76084-108">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos.</span><span class="sxs-lookup"><span data-stu-id="76084-108">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="76084-109">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="76084-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="76084-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="76084-110">Permissions</span></span>

<span data-ttu-id="76084-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76084-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76084-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76084-113">Permission type</span></span>                        | <span data-ttu-id="76084-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76084-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="76084-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76084-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="76084-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="76084-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="76084-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76084-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76084-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76084-118">Not supported.</span></span>                           |
| <span data-ttu-id="76084-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76084-119">Application</span></span>                            | <span data-ttu-id="76084-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="76084-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="76084-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76084-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="76084-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="76084-122">Function parameters</span></span>

<span data-ttu-id="76084-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="76084-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="76084-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="76084-124">Parameter</span></span> | <span data-ttu-id="76084-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="76084-125">Type</span></span>   | <span data-ttu-id="76084-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="76084-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="76084-127">ponto</span><span class="sxs-lookup"><span data-stu-id="76084-127">period</span></span>    | <span data-ttu-id="76084-128">string</span><span class="sxs-lookup"><span data-stu-id="76084-128">string</span></span> | <span data-ttu-id="76084-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="76084-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="76084-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="76084-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="76084-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="76084-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="76084-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76084-132">Required.</span></span> |

<span data-ttu-id="76084-133">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="76084-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="76084-134">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="76084-134">The default output type is text/csv.</span></span> <span data-ttu-id="76084-135">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="76084-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76084-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76084-136">Request headers</span></span>

| <span data-ttu-id="76084-137">Nome</span><span class="sxs-lookup"><span data-stu-id="76084-137">Name</span></span>          | <span data-ttu-id="76084-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="76084-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="76084-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="76084-139">Authorization</span></span> | <span data-ttu-id="76084-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76084-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="76084-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="76084-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="76084-143">CSV</span><span class="sxs-lookup"><span data-stu-id="76084-143">CSV</span></span>

<span data-ttu-id="76084-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="76084-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="76084-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="76084-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="76084-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="76084-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="76084-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="76084-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="76084-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="76084-148">Report Refresh Date</span></span>
- <span data-ttu-id="76084-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="76084-149">Report Date</span></span>
- <span data-ttu-id="76084-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="76084-150">Report Period</span></span>
- <span data-ttu-id="76084-151">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="76084-151">IM</span></span>
- <span data-ttu-id="76084-152">Áudio</span><span class="sxs-lookup"><span data-stu-id="76084-152">Audio</span></span>
- <span data-ttu-id="76084-153">Vídeo</span><span class="sxs-lookup"><span data-stu-id="76084-153">Video</span></span>
- <span data-ttu-id="76084-154">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="76084-154">App Sharing</span></span>
- <span data-ttu-id="76084-155">Transferência de arquivos</span><span class="sxs-lookup"><span data-stu-id="76084-155">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="76084-156">JSON</span><span class="sxs-lookup"><span data-stu-id="76084-156">JSON</span></span>

<span data-ttu-id="76084-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76084-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76084-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76084-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="76084-159">CSV</span><span class="sxs-lookup"><span data-stu-id="76084-159">CSV</span></span>

<span data-ttu-id="76084-160">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="76084-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="76084-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76084-161">Request</span></span>

<span data-ttu-id="76084-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="76084-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="76084-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="76084-163">Response</span></span>

<span data-ttu-id="76084-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="76084-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="76084-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="76084-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```

### <a name="json"></a><span data-ttu-id="76084-166">JSON</span><span class="sxs-lookup"><span data-stu-id="76084-166">JSON</span></span>

<span data-ttu-id="76084-167">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="76084-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="76084-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76084-168">Request</span></span>

<span data-ttu-id="76084-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="76084-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="76084-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="76084-170">Response</span></span>

<span data-ttu-id="76084-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="76084-171">The following is an example of the response.</span></span>

> <span data-ttu-id="76084-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76084-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityCounts)", 
  "value": [
    {
      "im": 1177, 
      "audio": 107, 
      "video": 7, 
      "appSharing": 74, 
      "fileTransfer": 24, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
