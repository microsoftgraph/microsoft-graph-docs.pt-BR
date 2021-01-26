---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 01dae8db1d6ab014e936395650c4f4291dfdd430
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983110"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="7f754-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="7f754-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="7f754-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f754-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7f754-105">Obtém o número de usuários exclusivos do Microsoft Teams por tipo de dispositivo no período de tempo selecionado.</span><span class="sxs-lookup"><span data-stu-id="7f754-105">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f754-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f754-106">Permissions</span></span>

<span data-ttu-id="7f754-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f754-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f754-109">Permission type</span></span>                        | <span data-ttu-id="7f754-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f754-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7f754-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f754-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f754-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f754-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7f754-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f754-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f754-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f754-114">Not supported.</span></span>                           |
| <span data-ttu-id="7f754-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f754-115">Application</span></span>                            | <span data-ttu-id="7f754-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f754-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="7f754-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="7f754-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7f754-118">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="7f754-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7f754-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f754-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7f754-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7f754-120">Function parameters</span></span>

<span data-ttu-id="7f754-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="7f754-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7f754-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7f754-122">Parameter</span></span> | <span data-ttu-id="7f754-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f754-123">Type</span></span>   | <span data-ttu-id="7f754-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f754-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7f754-125">ponto</span><span class="sxs-lookup"><span data-stu-id="7f754-125">period</span></span>    | <span data-ttu-id="7f754-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f754-126">string</span></span> | <span data-ttu-id="7f754-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7f754-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7f754-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="7f754-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7f754-129">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="7f754-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7f754-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f754-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7f754-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f754-131">Request headers</span></span>

| <span data-ttu-id="7f754-132">Nome</span><span class="sxs-lookup"><span data-stu-id="7f754-132">Name</span></span>          | <span data-ttu-id="7f754-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f754-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7f754-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f754-134">Authorization</span></span> | <span data-ttu-id="7f754-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f754-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7f754-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f754-137">Response</span></span>

<span data-ttu-id="7f754-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7f754-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7f754-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7f754-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7f754-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7f754-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7f754-141">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="7f754-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="7f754-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7f754-142">Report Refresh Date</span></span>
- <span data-ttu-id="7f754-143">Web</span><span class="sxs-lookup"><span data-stu-id="7f754-143">Web</span></span>
- <span data-ttu-id="7f754-144">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="7f754-144">Windows Phone</span></span>
- <span data-ttu-id="7f754-145">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="7f754-145">Android Phone</span></span>
- <span data-ttu-id="7f754-146">iOS</span><span class="sxs-lookup"><span data-stu-id="7f754-146">iOS</span></span>
- <span data-ttu-id="7f754-147">Mac</span><span class="sxs-lookup"><span data-stu-id="7f754-147">Mac</span></span>
- <span data-ttu-id="7f754-148">Windows</span><span class="sxs-lookup"><span data-stu-id="7f754-148">Windows</span></span>
- <span data-ttu-id="7f754-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="7f754-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7f754-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f754-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7f754-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f754-151">Request</span></span>

<span data-ttu-id="7f754-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f754-152">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="7f754-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f754-153">Response</span></span>

<span data-ttu-id="7f754-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f754-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7f754-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7f754-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
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

