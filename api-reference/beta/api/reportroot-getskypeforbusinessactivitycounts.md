---
title: 'reportRoot: getSkypeForBusinessActivityCounts'
description: Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 2d0336f3655160c678921c15d4a170df30343c4d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983808"
---
# <a name="reportroot-getskypeforbusinessactivitycounts"></a><span data-ttu-id="01d96-104">reportRoot: getSkypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="01d96-104">reportRoot: getSkypeForBusinessActivityCounts</span></span>

<span data-ttu-id="01d96-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01d96-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01d96-106">Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="01d96-106">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="01d96-107">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="01d96-107">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="01d96-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Microsoft 365 - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="01d96-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="01d96-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="01d96-109">Permissions</span></span>

<span data-ttu-id="01d96-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01d96-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01d96-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01d96-112">Permission type</span></span>                        | <span data-ttu-id="01d96-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01d96-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="01d96-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01d96-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="01d96-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="01d96-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="01d96-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01d96-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01d96-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01d96-117">Not supported.</span></span>                           |
| <span data-ttu-id="01d96-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01d96-118">Application</span></span>                            | <span data-ttu-id="01d96-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="01d96-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="01d96-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="01d96-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="01d96-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="01d96-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="01d96-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01d96-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="01d96-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="01d96-123">Function parameters</span></span>

<span data-ttu-id="01d96-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="01d96-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="01d96-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="01d96-125">Parameter</span></span> | <span data-ttu-id="01d96-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="01d96-126">Type</span></span>   | <span data-ttu-id="01d96-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="01d96-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="01d96-128">ponto</span><span class="sxs-lookup"><span data-stu-id="01d96-128">period</span></span>    | <span data-ttu-id="01d96-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01d96-129">string</span></span> | <span data-ttu-id="01d96-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="01d96-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="01d96-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="01d96-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="01d96-132">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="01d96-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="01d96-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01d96-133">Required.</span></span> |

<span data-ttu-id="01d96-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="01d96-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="01d96-135">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="01d96-135">The default output type is text/csv.</span></span> <span data-ttu-id="01d96-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="01d96-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01d96-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01d96-137">Request headers</span></span>

| <span data-ttu-id="01d96-138">Nome</span><span class="sxs-lookup"><span data-stu-id="01d96-138">Name</span></span>          | <span data-ttu-id="01d96-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="01d96-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="01d96-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="01d96-140">Authorization</span></span> | <span data-ttu-id="01d96-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01d96-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="01d96-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="01d96-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="01d96-144">CSV</span><span class="sxs-lookup"><span data-stu-id="01d96-144">CSV</span></span>

<span data-ttu-id="01d96-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="01d96-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="01d96-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="01d96-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="01d96-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="01d96-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="01d96-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="01d96-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="01d96-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="01d96-149">Report Refresh Date</span></span>
- <span data-ttu-id="01d96-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="01d96-150">Report Date</span></span>
- <span data-ttu-id="01d96-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="01d96-151">Report Period</span></span>
- <span data-ttu-id="01d96-152">Ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="01d96-152">Peer-to-peer</span></span>
- <span data-ttu-id="01d96-153">Organizadas</span><span class="sxs-lookup"><span data-stu-id="01d96-153">Organized</span></span>
- <span data-ttu-id="01d96-154">Participadas</span><span class="sxs-lookup"><span data-stu-id="01d96-154">Participated</span></span>

### <a name="json"></a><span data-ttu-id="01d96-155">JSON</span><span class="sxs-lookup"><span data-stu-id="01d96-155">JSON</span></span>

<span data-ttu-id="01d96-156">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` **[skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01d96-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01d96-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01d96-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="01d96-158">CSV</span><span class="sxs-lookup"><span data-stu-id="01d96-158">CSV</span></span>

<span data-ttu-id="01d96-159">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="01d96-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="01d96-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01d96-160">Request</span></span>

<span data-ttu-id="01d96-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01d96-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="01d96-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="01d96-162">Response</span></span>

<span data-ttu-id="01d96-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01d96-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="01d96-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="01d96-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```

### <a name="json"></a><span data-ttu-id="01d96-165">JSON</span><span class="sxs-lookup"><span data-stu-id="01d96-165">JSON</span></span>

<span data-ttu-id="01d96-166">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="01d96-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="01d96-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01d96-167">Request</span></span>

<span data-ttu-id="01d96-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01d96-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="01d96-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="01d96-169">Response</span></span>

<span data-ttu-id="01d96-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01d96-170">The following is an example of the response.</span></span>

> <span data-ttu-id="01d96-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01d96-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityCounts)", 
  "value": [
    {
      "peerToPeer": 3436, 
      "organized": 58, 
      "participated": 209, 
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


