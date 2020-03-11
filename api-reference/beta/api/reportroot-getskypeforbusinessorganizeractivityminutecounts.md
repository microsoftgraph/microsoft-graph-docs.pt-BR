---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 82f118cb2611b9c740c2a81a1ad26e3380907af2
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590435"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="1e02f-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="1e02f-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="1e02f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e02f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e02f-106">Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="1e02f-106">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="1e02f-107">Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1e02f-107">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="1e02f-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do organizador da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="1e02f-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e02f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e02f-109">Permissions</span></span>

<span data-ttu-id="1e02f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e02f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e02f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e02f-112">Permission type</span></span>                        | <span data-ttu-id="1e02f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e02f-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1e02f-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e02f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e02f-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e02f-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1e02f-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e02f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e02f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e02f-117">Not supported.</span></span>                           |
| <span data-ttu-id="1e02f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e02f-118">Application</span></span>                            | <span data-ttu-id="1e02f-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e02f-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="1e02f-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="1e02f-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="1e02f-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="1e02f-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="1e02f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e02f-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1e02f-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="1e02f-123">Function parameters</span></span>

<span data-ttu-id="1e02f-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1e02f-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1e02f-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1e02f-125">Parameter</span></span> | <span data-ttu-id="1e02f-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e02f-126">Type</span></span>   | <span data-ttu-id="1e02f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e02f-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1e02f-128">ponto</span><span class="sxs-lookup"><span data-stu-id="1e02f-128">period</span></span>    | <span data-ttu-id="1e02f-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e02f-129">string</span></span> | <span data-ttu-id="1e02f-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1e02f-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1e02f-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="1e02f-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1e02f-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1e02f-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1e02f-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e02f-133">Required.</span></span> |

<span data-ttu-id="1e02f-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1e02f-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1e02f-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="1e02f-135">The default output type is text/csv.</span></span> <span data-ttu-id="1e02f-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="1e02f-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e02f-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e02f-137">Request headers</span></span>

| <span data-ttu-id="1e02f-138">Nome</span><span class="sxs-lookup"><span data-stu-id="1e02f-138">Name</span></span>          | <span data-ttu-id="1e02f-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e02f-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1e02f-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e02f-140">Authorization</span></span> | <span data-ttu-id="1e02f-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e02f-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1e02f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e02f-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1e02f-144">CSV</span><span class="sxs-lookup"><span data-stu-id="1e02f-144">CSV</span></span>

<span data-ttu-id="1e02f-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="1e02f-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1e02f-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1e02f-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1e02f-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1e02f-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1e02f-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="1e02f-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1e02f-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="1e02f-149">Report Refresh Date</span></span>
- <span data-ttu-id="1e02f-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="1e02f-150">Report Date</span></span>
- <span data-ttu-id="1e02f-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="1e02f-151">Report Period</span></span>
- <span data-ttu-id="1e02f-152">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="1e02f-152">Audio/Video</span></span>
- <span data-ttu-id="1e02f-153">Dial-in pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="1e02f-153">Dial-in Microsoft</span></span>
- <span data-ttu-id="1e02f-154">Dial-out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="1e02f-154">Dial-out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="1e02f-155">JSON</span><span class="sxs-lookup"><span data-stu-id="1e02f-155">JSON</span></span>

<span data-ttu-id="1e02f-156">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e02f-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e02f-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e02f-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1e02f-158">CSV</span><span class="sxs-lookup"><span data-stu-id="1e02f-158">CSV</span></span>

<span data-ttu-id="1e02f-159">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="1e02f-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1e02f-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e02f-160">Request</span></span>

<span data-ttu-id="1e02f-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e02f-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="1e02f-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e02f-162">Response</span></span>

<span data-ttu-id="1e02f-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1e02f-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1e02f-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="1e02f-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
```

### <a name="json"></a><span data-ttu-id="1e02f-165">JSON</span><span class="sxs-lookup"><span data-stu-id="1e02f-165">JSON</span></span>

<span data-ttu-id="1e02f-166">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="1e02f-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1e02f-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e02f-167">Request</span></span>

<span data-ttu-id="1e02f-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e02f-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="1e02f-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e02f-169">Response</span></span>

<span data-ttu-id="1e02f-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1e02f-170">The following is an example of the response.</span></span>

> <span data-ttu-id="1e02f-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e02f-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts)", 
  "value": [
    {
      "audioVideo": 1912, 
      "dialInMicrosoft": 108, 
      "dialOutMicrosoft": 0, 
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
