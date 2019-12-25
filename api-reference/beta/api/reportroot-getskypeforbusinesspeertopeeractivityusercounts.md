---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f977054bff5e8c5cfc48048293f2518ea622cdc5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868937"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="679df-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="679df-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="679df-105">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="679df-105">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="679df-106">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="679df-106">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="679df-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="679df-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="679df-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="679df-108">Permissions</span></span>

<span data-ttu-id="679df-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="679df-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="679df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="679df-111">Permission type</span></span>                        | <span data-ttu-id="679df-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="679df-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="679df-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="679df-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="679df-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="679df-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="679df-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="679df-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="679df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="679df-116">Not supported.</span></span>                           |
| <span data-ttu-id="679df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="679df-117">Application</span></span>                            | <span data-ttu-id="679df-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="679df-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="679df-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="679df-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="679df-120">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="679df-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="679df-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="679df-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="679df-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="679df-122">Function parameters</span></span>

<span data-ttu-id="679df-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="679df-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="679df-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="679df-124">Parameter</span></span> | <span data-ttu-id="679df-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="679df-125">Type</span></span>   | <span data-ttu-id="679df-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="679df-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="679df-127">ponto</span><span class="sxs-lookup"><span data-stu-id="679df-127">period</span></span>    | <span data-ttu-id="679df-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="679df-128">string</span></span> | <span data-ttu-id="679df-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="679df-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="679df-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="679df-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="679df-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="679df-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="679df-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="679df-132">Required.</span></span> |

<span data-ttu-id="679df-133">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="679df-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="679df-134">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="679df-134">The default output type is text/csv.</span></span> <span data-ttu-id="679df-135">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="679df-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="679df-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="679df-136">Request headers</span></span>

| <span data-ttu-id="679df-137">Nome</span><span class="sxs-lookup"><span data-stu-id="679df-137">Name</span></span>          | <span data-ttu-id="679df-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="679df-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="679df-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="679df-139">Authorization</span></span> | <span data-ttu-id="679df-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="679df-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="679df-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="679df-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="679df-143">CSV</span><span class="sxs-lookup"><span data-stu-id="679df-143">CSV</span></span>

<span data-ttu-id="679df-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="679df-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="679df-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="679df-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="679df-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="679df-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="679df-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="679df-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="679df-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="679df-148">Report Refresh Date</span></span>
- <span data-ttu-id="679df-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="679df-149">Report Date</span></span>
- <span data-ttu-id="679df-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="679df-150">Report Period</span></span>
- <span data-ttu-id="679df-151">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="679df-151">IM</span></span>
- <span data-ttu-id="679df-152">Áudio</span><span class="sxs-lookup"><span data-stu-id="679df-152">Audio</span></span>
- <span data-ttu-id="679df-153">Vídeo</span><span class="sxs-lookup"><span data-stu-id="679df-153">Video</span></span>
- <span data-ttu-id="679df-154">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="679df-154">App Sharing</span></span>
- <span data-ttu-id="679df-155">Transferência de arquivos</span><span class="sxs-lookup"><span data-stu-id="679df-155">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="679df-156">JSON</span><span class="sxs-lookup"><span data-stu-id="679df-156">JSON</span></span>

<span data-ttu-id="679df-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="679df-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="679df-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="679df-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="679df-159">CSV</span><span class="sxs-lookup"><span data-stu-id="679df-159">CSV</span></span>

<span data-ttu-id="679df-160">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="679df-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="679df-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="679df-161">Request</span></span>

<span data-ttu-id="679df-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="679df-162">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="679df-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="679df-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="679df-164">C#</span><span class="sxs-lookup"><span data-stu-id="679df-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="679df-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="679df-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="679df-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="679df-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="679df-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="679df-167">Response</span></span>

<span data-ttu-id="679df-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="679df-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="679df-169">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="679df-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="679df-170">JSON</span><span class="sxs-lookup"><span data-stu-id="679df-170">JSON</span></span>

<span data-ttu-id="679df-171">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="679df-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="679df-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="679df-172">Request</span></span>

<span data-ttu-id="679df-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="679df-173">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="679df-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="679df-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="679df-175">C#</span><span class="sxs-lookup"><span data-stu-id="679df-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="679df-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="679df-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="679df-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="679df-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="679df-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="679df-178">Response</span></span>

<span data-ttu-id="679df-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="679df-179">The following is an example of the response.</span></span>

> <span data-ttu-id="679df-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="679df-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts)", 
  "value": [
    {
      "im": 379, 
      "audio": 42, 
      "video": 2, 
      "appSharing": 34, 
      "fileTransfer": 36, 
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
