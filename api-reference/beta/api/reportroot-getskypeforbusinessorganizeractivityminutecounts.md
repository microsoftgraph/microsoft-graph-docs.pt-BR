---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: e795e0b566bf5d23b1ebdadb6c4d3e7d2a4d81ca
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052800"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="f72cf-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="f72cf-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="f72cf-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f72cf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f72cf-106">Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="f72cf-106">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="f72cf-107">Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f72cf-107">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="f72cf-108">**Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, consulte Microsoft 365 relatórios - Skype for Business atividade do organizador [da conferência.](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)</span><span class="sxs-lookup"><span data-stu-id="f72cf-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="f72cf-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f72cf-109">Permissions</span></span>

<span data-ttu-id="f72cf-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f72cf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f72cf-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f72cf-112">Permission type</span></span>                        | <span data-ttu-id="f72cf-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f72cf-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f72cf-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f72cf-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f72cf-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f72cf-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f72cf-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f72cf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f72cf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f72cf-117">Not supported.</span></span>                           |
| <span data-ttu-id="f72cf-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f72cf-118">Application</span></span>                            | <span data-ttu-id="f72cf-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f72cf-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="f72cf-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="f72cf-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="f72cf-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="f72cf-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="f72cf-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f72cf-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f72cf-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f72cf-123">Function parameters</span></span>

<span data-ttu-id="f72cf-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="f72cf-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f72cf-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f72cf-125">Parameter</span></span> | <span data-ttu-id="f72cf-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="f72cf-126">Type</span></span>   | <span data-ttu-id="f72cf-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f72cf-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f72cf-128">ponto</span><span class="sxs-lookup"><span data-stu-id="f72cf-128">period</span></span>    | <span data-ttu-id="f72cf-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f72cf-129">string</span></span> | <span data-ttu-id="f72cf-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f72cf-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f72cf-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f72cf-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f72cf-132">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f72cf-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f72cf-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f72cf-133">Required.</span></span> |

<span data-ttu-id="f72cf-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f72cf-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f72cf-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="f72cf-135">The default output type is text/csv.</span></span> <span data-ttu-id="f72cf-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="f72cf-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f72cf-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f72cf-137">Request headers</span></span>

| <span data-ttu-id="f72cf-138">Nome</span><span class="sxs-lookup"><span data-stu-id="f72cf-138">Name</span></span>          | <span data-ttu-id="f72cf-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="f72cf-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f72cf-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="f72cf-140">Authorization</span></span> | <span data-ttu-id="f72cf-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f72cf-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f72cf-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f72cf-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f72cf-144">CSV</span><span class="sxs-lookup"><span data-stu-id="f72cf-144">CSV</span></span>

<span data-ttu-id="f72cf-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f72cf-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f72cf-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f72cf-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f72cf-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f72cf-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f72cf-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f72cf-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f72cf-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f72cf-149">Report Refresh Date</span></span>
- <span data-ttu-id="f72cf-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="f72cf-150">Report Date</span></span>
- <span data-ttu-id="f72cf-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f72cf-151">Report Period</span></span>
- <span data-ttu-id="f72cf-152">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="f72cf-152">Audio/Video</span></span>
- <span data-ttu-id="f72cf-153">Dial-in pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="f72cf-153">Dial-in Microsoft</span></span>
- <span data-ttu-id="f72cf-154">Dial-out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="f72cf-154">Dial-out Microsoft</span></span>

### <a name="json"></a><span data-ttu-id="f72cf-155">JSON</span><span class="sxs-lookup"><span data-stu-id="f72cf-155">JSON</span></span>

<span data-ttu-id="f72cf-156">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f72cf-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f72cf-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f72cf-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f72cf-158">CSV</span><span class="sxs-lookup"><span data-stu-id="f72cf-158">CSV</span></span>

<span data-ttu-id="f72cf-159">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="f72cf-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f72cf-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f72cf-160">Request</span></span>

<span data-ttu-id="f72cf-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f72cf-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="f72cf-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="f72cf-162">Response</span></span>

<span data-ttu-id="f72cf-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f72cf-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f72cf-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f72cf-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="f72cf-165">JSON</span><span class="sxs-lookup"><span data-stu-id="f72cf-165">JSON</span></span>

<span data-ttu-id="f72cf-166">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="f72cf-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f72cf-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f72cf-167">Request</span></span>

<span data-ttu-id="f72cf-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f72cf-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="f72cf-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="f72cf-169">Response</span></span>

<span data-ttu-id="f72cf-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f72cf-170">The following is an example of the response.</span></span>

> <span data-ttu-id="f72cf-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f72cf-171">**Note:** The response object shown here might be shortened for readability.</span></span>

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


