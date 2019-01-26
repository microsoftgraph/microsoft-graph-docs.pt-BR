---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business. Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 980e83838833e2fc7c16218417eb84df4949cc83
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572084"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="f684c-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="f684c-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="f684c-105">Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="f684c-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="f684c-106">Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.</span><span class="sxs-lookup"><span data-stu-id="f684c-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="f684c-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="f684c-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="f684c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f684c-108">Permissions</span></span>

<span data-ttu-id="f684c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f684c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f684c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f684c-111">Permission type</span></span>                        | <span data-ttu-id="f684c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f684c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f684c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f684c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f684c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f684c-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f684c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f684c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f684c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f684c-116">Not supported.</span></span>                           |
| <span data-ttu-id="f684c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f684c-117">Application</span></span>                            | <span data-ttu-id="f684c-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f684c-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f684c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f684c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f684c-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f684c-120">Function parameters</span></span>

<span data-ttu-id="f684c-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="f684c-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f684c-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f684c-122">Parameter</span></span> | <span data-ttu-id="f684c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f684c-123">Type</span></span>   | <span data-ttu-id="f684c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f684c-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f684c-125">ponto</span><span class="sxs-lookup"><span data-stu-id="f684c-125">period</span></span>    | <span data-ttu-id="f684c-126">string</span><span class="sxs-lookup"><span data-stu-id="f684c-126">string</span></span> | <span data-ttu-id="f684c-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f684c-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f684c-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f684c-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f684c-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f684c-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f684c-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f684c-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f684c-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f684c-131">Request headers</span></span>

| <span data-ttu-id="f684c-132">Nome</span><span class="sxs-lookup"><span data-stu-id="f684c-132">Name</span></span>          | <span data-ttu-id="f684c-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f684c-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f684c-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="f684c-134">Authorization</span></span> | <span data-ttu-id="f684c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f684c-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f684c-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f684c-137">If-None-Match</span></span> | <span data-ttu-id="f684c-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="f684c-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f684c-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f684c-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f684c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f684c-140">Response</span></span>

<span data-ttu-id="f684c-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f684c-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f684c-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f684c-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f684c-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f684c-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f684c-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f684c-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f684c-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f684c-145">Report Refresh Date</span></span>
- <span data-ttu-id="f684c-146">Windows</span><span class="sxs-lookup"><span data-stu-id="f684c-146">Windows</span></span>
- <span data-ttu-id="f684c-147">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="f684c-147">Windows Phone</span></span>
- <span data-ttu-id="f684c-148">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="f684c-148">Android Phone</span></span>
- <span data-ttu-id="f684c-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="f684c-149">iPhone</span></span>
- <span data-ttu-id="f684c-150">iPad</span><span class="sxs-lookup"><span data-stu-id="f684c-150">iPad</span></span>
- <span data-ttu-id="f684c-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="f684c-151">Report Date</span></span>
- <span data-ttu-id="f684c-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f684c-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f684c-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f684c-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f684c-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f684c-154">Request</span></span>

<span data-ttu-id="f684c-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f684c-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f684c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="f684c-156">Response</span></span>

<span data-ttu-id="f684c-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f684c-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="f684c-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f684c-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```
