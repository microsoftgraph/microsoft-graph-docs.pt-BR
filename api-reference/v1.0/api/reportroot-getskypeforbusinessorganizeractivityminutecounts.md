---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 89d5f9c277399e5189031a838ed00082bc4a4c0c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580810"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="9a405-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="9a405-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="9a405-105">Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="9a405-105">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="9a405-106">Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9a405-106">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="9a405-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do organizador da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="9a405-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a405-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a405-108">Permissions</span></span>

<span data-ttu-id="9a405-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a405-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a405-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a405-111">Permission type</span></span>                        | <span data-ttu-id="9a405-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a405-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9a405-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a405-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a405-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a405-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9a405-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a405-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a405-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a405-116">Not supported.</span></span>                           |
| <span data-ttu-id="9a405-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a405-117">Application</span></span>                            | <span data-ttu-id="9a405-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a405-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9a405-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a405-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9a405-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9a405-120">Function parameters</span></span>

<span data-ttu-id="9a405-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="9a405-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9a405-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9a405-122">Parameter</span></span> | <span data-ttu-id="9a405-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a405-123">Type</span></span>   | <span data-ttu-id="9a405-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a405-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9a405-125">ponto</span><span class="sxs-lookup"><span data-stu-id="9a405-125">period</span></span>    | <span data-ttu-id="9a405-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a405-126">string</span></span> | <span data-ttu-id="9a405-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9a405-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9a405-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9a405-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9a405-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9a405-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9a405-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a405-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9a405-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a405-131">Request headers</span></span>

| <span data-ttu-id="9a405-132">Nome</span><span class="sxs-lookup"><span data-stu-id="9a405-132">Name</span></span>          | <span data-ttu-id="9a405-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a405-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="9a405-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a405-134">Authorization</span></span> | <span data-ttu-id="9a405-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a405-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="9a405-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="9a405-137">If-None-Match</span></span> | <span data-ttu-id="9a405-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="9a405-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="9a405-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9a405-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="9a405-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a405-140">Response</span></span>

<span data-ttu-id="9a405-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9a405-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9a405-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9a405-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9a405-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9a405-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9a405-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="9a405-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9a405-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9a405-145">Report Refresh Date</span></span>
- <span data-ttu-id="9a405-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="9a405-146">Report Date</span></span>
- <span data-ttu-id="9a405-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9a405-147">Report Period</span></span>
- <span data-ttu-id="9a405-148">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="9a405-148">Audio/Video</span></span>
- <span data-ttu-id="9a405-149">Dial-in pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="9a405-149">Dial-in Microsoft</span></span>
- <span data-ttu-id="9a405-150">Dial-out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="9a405-150">Dial-out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="9a405-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a405-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9a405-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a405-152">Request</span></span>

<span data-ttu-id="9a405-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a405-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="9a405-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a405-154">Response</span></span>

<span data-ttu-id="9a405-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a405-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="9a405-156">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9a405-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
```
