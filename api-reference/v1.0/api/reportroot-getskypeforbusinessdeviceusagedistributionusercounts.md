---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Obtenha o número de usuários que usam dispositivos exclusivos em sua organização. O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3282532aba58c63c210d8f58ab96b7313a9b2910
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954889"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="8d3de-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="8d3de-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="8d3de-105">Obtenha o número de usuários que usam dispositivos exclusivos em sua organização.</span><span class="sxs-lookup"><span data-stu-id="8d3de-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="8d3de-106">O relatório mostrará o número de usuários por dispositivo, incluindo Windows, Windows Phone, telefone Android, iPhone e iPad.</span><span class="sxs-lookup"><span data-stu-id="8d3de-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="8d3de-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="8d3de-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d3de-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d3de-108">Permissions</span></span>

<span data-ttu-id="8d3de-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d3de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d3de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d3de-111">Permission type</span></span>                        | <span data-ttu-id="8d3de-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d3de-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8d3de-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d3de-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d3de-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d3de-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8d3de-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d3de-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d3de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d3de-116">Not supported.</span></span>                           |
| <span data-ttu-id="8d3de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d3de-117">Application</span></span>                            | <span data-ttu-id="8d3de-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d3de-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8d3de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d3de-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8d3de-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8d3de-120">Function parameters</span></span>

<span data-ttu-id="8d3de-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="8d3de-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8d3de-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8d3de-122">Parameter</span></span> | <span data-ttu-id="8d3de-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d3de-123">Type</span></span>   | <span data-ttu-id="8d3de-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d3de-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8d3de-125">ponto</span><span class="sxs-lookup"><span data-stu-id="8d3de-125">period</span></span>    | <span data-ttu-id="8d3de-126">string</span><span class="sxs-lookup"><span data-stu-id="8d3de-126">string</span></span> | <span data-ttu-id="8d3de-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8d3de-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8d3de-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="8d3de-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8d3de-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8d3de-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8d3de-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d3de-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8d3de-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d3de-131">Request headers</span></span>

| <span data-ttu-id="8d3de-132">Nome</span><span class="sxs-lookup"><span data-stu-id="8d3de-132">Name</span></span>          | <span data-ttu-id="8d3de-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d3de-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8d3de-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d3de-134">Authorization</span></span> | <span data-ttu-id="8d3de-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d3de-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8d3de-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8d3de-137">If-None-Match</span></span> | <span data-ttu-id="8d3de-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="8d3de-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8d3de-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8d3de-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8d3de-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d3de-140">Response</span></span>

<span data-ttu-id="8d3de-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="8d3de-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8d3de-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="8d3de-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8d3de-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8d3de-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8d3de-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="8d3de-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8d3de-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="8d3de-145">Report Refresh Date</span></span>
- <span data-ttu-id="8d3de-146">Windows</span><span class="sxs-lookup"><span data-stu-id="8d3de-146">Windows</span></span>
- <span data-ttu-id="8d3de-147">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="8d3de-147">Windows Phone</span></span>
- <span data-ttu-id="8d3de-148">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="8d3de-148">Android Phone</span></span>
- <span data-ttu-id="8d3de-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="8d3de-149">iPhone</span></span>
- <span data-ttu-id="8d3de-150">iPad</span><span class="sxs-lookup"><span data-stu-id="8d3de-150">iPad</span></span>
- <span data-ttu-id="8d3de-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="8d3de-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8d3de-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d3de-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8d3de-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d3de-153">Request</span></span>

<span data-ttu-id="8d3de-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d3de-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8d3de-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d3de-155">Response</span></span>

<span data-ttu-id="8d3de-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d3de-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="8d3de-157">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="8d3de-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```
