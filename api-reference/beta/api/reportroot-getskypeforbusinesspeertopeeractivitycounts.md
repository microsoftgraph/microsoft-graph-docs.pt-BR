---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityCounts'
description: Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 772bbd5486e9141b6627ce0c8dbab97d289dbcaa
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896193"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="5a1eb-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="5a1eb-104">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

<span data-ttu-id="5a1eb-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a1eb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a1eb-106">Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-106">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="5a1eb-107">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-107">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="5a1eb-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Skype for Business peer-to-peer Activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="5a1eb-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="5a1eb-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a1eb-109">Permissions</span></span>

<span data-ttu-id="5a1eb-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5a1eb-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a1eb-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a1eb-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a1eb-112">Permission type</span></span>                        | <span data-ttu-id="5a1eb-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a1eb-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5a1eb-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a1eb-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a1eb-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a1eb-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5a1eb-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a1eb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a1eb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-117">Not supported.</span></span>                           |
| <span data-ttu-id="5a1eb-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a1eb-118">Application</span></span>                            | <span data-ttu-id="5a1eb-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a1eb-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="5a1eb-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5a1eb-121">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5a1eb-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5a1eb-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a1eb-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5a1eb-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5a1eb-123">Function parameters</span></span>

<span data-ttu-id="5a1eb-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5a1eb-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5a1eb-125">Parameter</span></span> | <span data-ttu-id="5a1eb-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a1eb-126">Type</span></span>   | <span data-ttu-id="5a1eb-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a1eb-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5a1eb-128">ponto</span><span class="sxs-lookup"><span data-stu-id="5a1eb-128">period</span></span>    | <span data-ttu-id="5a1eb-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a1eb-129">string</span></span> | <span data-ttu-id="5a1eb-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5a1eb-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5a1eb-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5a1eb-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-133">Required.</span></span> |

<span data-ttu-id="5a1eb-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5a1eb-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-135">The default output type is text/csv.</span></span> <span data-ttu-id="5a1eb-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a1eb-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a1eb-137">Request headers</span></span>

| <span data-ttu-id="5a1eb-138">Nome</span><span class="sxs-lookup"><span data-stu-id="5a1eb-138">Name</span></span>          | <span data-ttu-id="5a1eb-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a1eb-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5a1eb-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a1eb-140">Authorization</span></span> | <span data-ttu-id="5a1eb-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-141">Bearer {token}.</span></span> <span data-ttu-id="5a1eb-142">Required.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-142">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5a1eb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a1eb-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5a1eb-144">CSV</span><span class="sxs-lookup"><span data-stu-id="5a1eb-144">CSV</span></span>

<span data-ttu-id="5a1eb-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5a1eb-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5a1eb-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5a1eb-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5a1eb-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5a1eb-149">Report Refresh Date</span></span>
- <span data-ttu-id="5a1eb-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="5a1eb-150">Report Date</span></span>
- <span data-ttu-id="5a1eb-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5a1eb-151">Report Period</span></span>
- <span data-ttu-id="5a1eb-152">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="5a1eb-152">IM</span></span>
- <span data-ttu-id="5a1eb-153">Áudio</span><span class="sxs-lookup"><span data-stu-id="5a1eb-153">Audio</span></span>
- <span data-ttu-id="5a1eb-154">Vídeo</span><span class="sxs-lookup"><span data-stu-id="5a1eb-154">Video</span></span>
- <span data-ttu-id="5a1eb-155">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="5a1eb-155">App Sharing</span></span>
- <span data-ttu-id="5a1eb-156">Transferência de arquivos</span><span class="sxs-lookup"><span data-stu-id="5a1eb-156">File Transfer</span></span>

### <a name="json"></a><span data-ttu-id="5a1eb-157">JSON</span><span class="sxs-lookup"><span data-stu-id="5a1eb-157">JSON</span></span>

<span data-ttu-id="5a1eb-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a1eb-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a1eb-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5a1eb-160">CSV</span><span class="sxs-lookup"><span data-stu-id="5a1eb-160">CSV</span></span>

<span data-ttu-id="5a1eb-161">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5a1eb-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a1eb-162">Request</span></span>

<span data-ttu-id="5a1eb-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="5a1eb-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a1eb-164">Response</span></span>

<span data-ttu-id="5a1eb-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5a1eb-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5a1eb-167">JSON</span><span class="sxs-lookup"><span data-stu-id="5a1eb-167">JSON</span></span>

<span data-ttu-id="5a1eb-168">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5a1eb-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a1eb-169">Request</span></span>

<span data-ttu-id="5a1eb-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="5a1eb-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a1eb-171">Response</span></span>

<span data-ttu-id="5a1eb-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-172">The following is an example of the response.</span></span>

> <span data-ttu-id="5a1eb-173">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-173">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5a1eb-174">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5a1eb-174">All the properties will be returned from an actual call.</span></span>

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
