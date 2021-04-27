---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts'
description: Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização. Tipos de sessões incluem áudio e vídeo.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: ace9f2bbd8f6afe6b1db67b432f20e98ef7686e0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052758"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="41bf5-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="41bf5-104">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="41bf5-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41bf5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41bf5-106">Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="41bf5-106">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="41bf5-107">Tipos de sessões incluem áudio e vídeo.</span><span class="sxs-lookup"><span data-stu-id="41bf5-107">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="41bf5-108">**Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Skype for Business atividade ponto a ponto](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="41bf5-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="41bf5-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="41bf5-109">Permissions</span></span>

<span data-ttu-id="41bf5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41bf5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41bf5-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41bf5-112">Permission type</span></span>                        | <span data-ttu-id="41bf5-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41bf5-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="41bf5-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41bf5-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="41bf5-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="41bf5-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="41bf5-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41bf5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41bf5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41bf5-117">Not supported.</span></span>                           |
| <span data-ttu-id="41bf5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41bf5-118">Application</span></span>                            | <span data-ttu-id="41bf5-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="41bf5-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="41bf5-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="41bf5-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="41bf5-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="41bf5-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="41bf5-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41bf5-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="41bf5-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="41bf5-123">Function parameters</span></span>

<span data-ttu-id="41bf5-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="41bf5-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="41bf5-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="41bf5-125">Parameter</span></span> | <span data-ttu-id="41bf5-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="41bf5-126">Type</span></span>   | <span data-ttu-id="41bf5-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="41bf5-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="41bf5-128">ponto</span><span class="sxs-lookup"><span data-stu-id="41bf5-128">period</span></span>    | <span data-ttu-id="41bf5-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41bf5-129">string</span></span> | <span data-ttu-id="41bf5-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="41bf5-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="41bf5-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="41bf5-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="41bf5-132">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="41bf5-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="41bf5-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41bf5-133">Required.</span></span> |

<span data-ttu-id="41bf5-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="41bf5-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="41bf5-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="41bf5-135">The default output type is text/csv.</span></span> <span data-ttu-id="41bf5-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="41bf5-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41bf5-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41bf5-137">Request headers</span></span>

| <span data-ttu-id="41bf5-138">Nome</span><span class="sxs-lookup"><span data-stu-id="41bf5-138">Name</span></span>          | <span data-ttu-id="41bf5-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="41bf5-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="41bf5-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="41bf5-140">Authorization</span></span> | <span data-ttu-id="41bf5-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41bf5-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="41bf5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="41bf5-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="41bf5-144">CSV</span><span class="sxs-lookup"><span data-stu-id="41bf5-144">CSV</span></span>

<span data-ttu-id="41bf5-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="41bf5-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="41bf5-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="41bf5-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="41bf5-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="41bf5-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="41bf5-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="41bf5-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="41bf5-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="41bf5-149">Report Refresh Date</span></span>
- <span data-ttu-id="41bf5-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="41bf5-150">Report Date</span></span>
- <span data-ttu-id="41bf5-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="41bf5-151">Report Period</span></span>
- <span data-ttu-id="41bf5-152">Áudio</span><span class="sxs-lookup"><span data-stu-id="41bf5-152">Audio</span></span>
- <span data-ttu-id="41bf5-153">Vídeo</span><span class="sxs-lookup"><span data-stu-id="41bf5-153">Video</span></span>

### <a name="json"></a><span data-ttu-id="41bf5-154">JSON</span><span class="sxs-lookup"><span data-stu-id="41bf5-154">JSON</span></span>

<span data-ttu-id="41bf5-155">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41bf5-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41bf5-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41bf5-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="41bf5-157">CSV</span><span class="sxs-lookup"><span data-stu-id="41bf5-157">CSV</span></span>

<span data-ttu-id="41bf5-158">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="41bf5-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="41bf5-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41bf5-159">Request</span></span>

<span data-ttu-id="41bf5-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41bf5-160">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="41bf5-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="41bf5-161">Response</span></span>

<span data-ttu-id="41bf5-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41bf5-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="41bf5-163">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="41bf5-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="41bf5-164">JSON</span><span class="sxs-lookup"><span data-stu-id="41bf5-164">JSON</span></span>

<span data-ttu-id="41bf5-165">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="41bf5-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="41bf5-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41bf5-166">Request</span></span>

<span data-ttu-id="41bf5-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41bf5-167">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="41bf5-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="41bf5-168">Response</span></span>

<span data-ttu-id="41bf5-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41bf5-169">The following is an example of the response.</span></span>

> <span data-ttu-id="41bf5-170">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="41bf5-170">**Note:** The response object shown here might be shortened for readability.</span></span>

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


