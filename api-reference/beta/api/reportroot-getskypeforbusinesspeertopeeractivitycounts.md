---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a260121c66a8aff080a39d0f581c20a4fc240cad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454073"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="4bbe2-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4bbe2-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

<span data-ttu-id="4bbe2-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4bbe2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bbe2-106">Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-106">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="4bbe2-107">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-107">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="4bbe2-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="4bbe2-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="4bbe2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4bbe2-109">Permissions</span></span>

<span data-ttu-id="4bbe2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bbe2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4bbe2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bbe2-112">Permission type</span></span>                        | <span data-ttu-id="4bbe2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bbe2-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4bbe2-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bbe2-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4bbe2-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bbe2-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4bbe2-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bbe2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bbe2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-117">Not supported.</span></span>                           |
| <span data-ttu-id="4bbe2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bbe2-118">Application</span></span>                            | <span data-ttu-id="4bbe2-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bbe2-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="4bbe2-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4bbe2-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="4bbe2-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4bbe2-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bbe2-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4bbe2-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4bbe2-123">Function parameters</span></span>

<span data-ttu-id="4bbe2-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4bbe2-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4bbe2-125">Parameter</span></span> | <span data-ttu-id="4bbe2-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bbe2-126">Type</span></span>   | <span data-ttu-id="4bbe2-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bbe2-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4bbe2-128">ponto</span><span class="sxs-lookup"><span data-stu-id="4bbe2-128">period</span></span>    | <span data-ttu-id="4bbe2-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bbe2-129">string</span></span> | <span data-ttu-id="4bbe2-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4bbe2-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4bbe2-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4bbe2-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-133">Required.</span></span> |

<span data-ttu-id="4bbe2-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4bbe2-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-135">The default output type is text/csv.</span></span> <span data-ttu-id="4bbe2-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bbe2-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bbe2-137">Request headers</span></span>

| <span data-ttu-id="4bbe2-138">Nome</span><span class="sxs-lookup"><span data-stu-id="4bbe2-138">Name</span></span>          | <span data-ttu-id="4bbe2-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bbe2-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4bbe2-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bbe2-140">Authorization</span></span> | <span data-ttu-id="4bbe2-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4bbe2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bbe2-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4bbe2-144">CSV</span><span class="sxs-lookup"><span data-stu-id="4bbe2-144">CSV</span></span>

<span data-ttu-id="4bbe2-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4bbe2-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4bbe2-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4bbe2-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4bbe2-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="4bbe2-149">Report Refresh Date</span></span>
- <span data-ttu-id="4bbe2-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="4bbe2-150">Report Date</span></span>
- <span data-ttu-id="4bbe2-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="4bbe2-151">Report Period</span></span>
- <span data-ttu-id="4bbe2-152">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="4bbe2-152">IM</span></span>
- <span data-ttu-id="4bbe2-153">Áudio</span><span class="sxs-lookup"><span data-stu-id="4bbe2-153">Audio</span></span>
- <span data-ttu-id="4bbe2-154">Vídeo</span><span class="sxs-lookup"><span data-stu-id="4bbe2-154">Video</span></span>
- <span data-ttu-id="4bbe2-155">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="4bbe2-155">App Sharing</span></span>
- <span data-ttu-id="4bbe2-156">Transferência de arquivos</span><span class="sxs-lookup"><span data-stu-id="4bbe2-156">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="4bbe2-157">JSON</span><span class="sxs-lookup"><span data-stu-id="4bbe2-157">JSON</span></span>

<span data-ttu-id="4bbe2-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bbe2-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bbe2-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4bbe2-160">CSV</span><span class="sxs-lookup"><span data-stu-id="4bbe2-160">CSV</span></span>

<span data-ttu-id="4bbe2-161">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4bbe2-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bbe2-162">Request</span></span>

<span data-ttu-id="4bbe2-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4bbe2-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bbe2-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="4bbe2-165">C#</span><span class="sxs-lookup"><span data-stu-id="4bbe2-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4bbe2-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bbe2-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4bbe2-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4bbe2-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4bbe2-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bbe2-168">Response</span></span>

<span data-ttu-id="4bbe2-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4bbe2-170">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4bbe2-171">JSON</span><span class="sxs-lookup"><span data-stu-id="4bbe2-171">JSON</span></span>

<span data-ttu-id="4bbe2-172">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4bbe2-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bbe2-173">Request</span></span>

<span data-ttu-id="4bbe2-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4bbe2-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bbe2-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="4bbe2-176">C#</span><span class="sxs-lookup"><span data-stu-id="4bbe2-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4bbe2-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4bbe2-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4bbe2-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4bbe2-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4bbe2-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bbe2-179">Response</span></span>

<span data-ttu-id="4bbe2-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-180">The following is an example of the response.</span></span>

> <span data-ttu-id="4bbe2-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bbe2-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
