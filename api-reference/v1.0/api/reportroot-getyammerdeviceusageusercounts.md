---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Obtenha o número de usuários diários por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: ec139af8abeff34d9a44bf37612455abbb1441bf
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983346"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="6fdae-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="6fdae-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="6fdae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fdae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fdae-105">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6fdae-105">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="6fdae-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, confira [relatórios do Microsoft 365 - uso de dispositivos do Yammer.](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)</span><span class="sxs-lookup"><span data-stu-id="6fdae-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="6fdae-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fdae-107">Permissions</span></span>

<span data-ttu-id="6fdae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fdae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6fdae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fdae-110">Permission type</span></span>                        | <span data-ttu-id="6fdae-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fdae-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6fdae-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fdae-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fdae-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6fdae-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6fdae-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fdae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fdae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fdae-115">Not supported.</span></span>                           |
| <span data-ttu-id="6fdae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fdae-116">Application</span></span>                            | <span data-ttu-id="6fdae-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6fdae-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="6fdae-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="6fdae-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="6fdae-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="6fdae-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="6fdae-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fdae-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6fdae-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="6fdae-121">Function parameters</span></span>

<span data-ttu-id="6fdae-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="6fdae-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6fdae-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6fdae-123">Parameter</span></span> | <span data-ttu-id="6fdae-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fdae-124">Type</span></span>   | <span data-ttu-id="6fdae-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fdae-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6fdae-126">ponto</span><span class="sxs-lookup"><span data-stu-id="6fdae-126">period</span></span>    | <span data-ttu-id="6fdae-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fdae-127">string</span></span> | <span data-ttu-id="6fdae-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6fdae-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6fdae-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="6fdae-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6fdae-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6fdae-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6fdae-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fdae-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6fdae-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fdae-132">Request headers</span></span>

| <span data-ttu-id="6fdae-133">Nome</span><span class="sxs-lookup"><span data-stu-id="6fdae-133">Name</span></span>          | <span data-ttu-id="6fdae-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fdae-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6fdae-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fdae-135">Authorization</span></span> | <span data-ttu-id="6fdae-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fdae-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6fdae-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6fdae-138">If-None-Match</span></span> | <span data-ttu-id="6fdae-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="6fdae-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6fdae-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6fdae-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6fdae-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fdae-141">Response</span></span>

<span data-ttu-id="6fdae-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="6fdae-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6fdae-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="6fdae-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6fdae-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6fdae-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6fdae-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="6fdae-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6fdae-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="6fdae-146">Report Refresh Date</span></span>
- <span data-ttu-id="6fdae-147">Web</span><span class="sxs-lookup"><span data-stu-id="6fdae-147">Web</span></span>
- <span data-ttu-id="6fdae-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="6fdae-148">Windows Phone</span></span>
- <span data-ttu-id="6fdae-149">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="6fdae-149">Android Phone</span></span>
- <span data-ttu-id="6fdae-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="6fdae-150">iPhone</span></span>
- <span data-ttu-id="6fdae-151">iPad</span><span class="sxs-lookup"><span data-stu-id="6fdae-151">iPad</span></span>
- <span data-ttu-id="6fdae-152">Outro</span><span class="sxs-lookup"><span data-stu-id="6fdae-152">Other</span></span>
- <span data-ttu-id="6fdae-153">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="6fdae-153">Report Date</span></span>
- <span data-ttu-id="6fdae-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="6fdae-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="6fdae-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fdae-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6fdae-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fdae-156">Request</span></span>

<span data-ttu-id="6fdae-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fdae-157">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="6fdae-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fdae-158">Response</span></span>

<span data-ttu-id="6fdae-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6fdae-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="6fdae-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="6fdae-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
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

