---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ae1dc1cd7272d1dc162f34560ab966bab2734e77
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554622"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="135a5-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="135a5-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="135a5-105">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="135a5-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="135a5-106">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="135a5-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="135a5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="135a5-107">Permissions</span></span>

<span data-ttu-id="135a5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="135a5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="135a5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="135a5-110">Permission type</span></span>                        | <span data-ttu-id="135a5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="135a5-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="135a5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="135a5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="135a5-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="135a5-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="135a5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="135a5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="135a5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="135a5-115">Not supported.</span></span>                           |
| <span data-ttu-id="135a5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="135a5-116">Application</span></span>                            | <span data-ttu-id="135a5-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="135a5-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="135a5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="135a5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="135a5-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="135a5-119">Function parameters</span></span>

<span data-ttu-id="135a5-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="135a5-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="135a5-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="135a5-121">Parameter</span></span> | <span data-ttu-id="135a5-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="135a5-122">Type</span></span>   | <span data-ttu-id="135a5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="135a5-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="135a5-124">ponto</span><span class="sxs-lookup"><span data-stu-id="135a5-124">period</span></span>    | <span data-ttu-id="135a5-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="135a5-125">string</span></span> | <span data-ttu-id="135a5-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="135a5-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="135a5-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="135a5-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="135a5-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="135a5-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="135a5-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="135a5-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="135a5-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="135a5-130">Request headers</span></span>

| <span data-ttu-id="135a5-131">Nome</span><span class="sxs-lookup"><span data-stu-id="135a5-131">Name</span></span>          | <span data-ttu-id="135a5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="135a5-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="135a5-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="135a5-133">Authorization</span></span> | <span data-ttu-id="135a5-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="135a5-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="135a5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="135a5-136">Response</span></span>

<span data-ttu-id="135a5-137">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="135a5-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="135a5-138">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="135a5-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="135a5-139">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="135a5-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="135a5-140">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="135a5-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="135a5-141">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="135a5-141">Report Refresh Date</span></span>
- <span data-ttu-id="135a5-142">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="135a5-142">Report Date</span></span>
- <span data-ttu-id="135a5-143">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="135a5-143">Team Chat Messages</span></span>
- <span data-ttu-id="135a5-144">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="135a5-144">Private Chat Messages</span></span>
- <span data-ttu-id="135a5-145">Chamadas</span><span class="sxs-lookup"><span data-stu-id="135a5-145">Calls</span></span>
- <span data-ttu-id="135a5-146">Reuniões</span><span class="sxs-lookup"><span data-stu-id="135a5-146">Meetings</span></span>
- <span data-ttu-id="135a5-147">Outras Ações</span><span class="sxs-lookup"><span data-stu-id="135a5-147">Other Actions</span></span>
- <span data-ttu-id="135a5-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="135a5-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="135a5-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="135a5-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="135a5-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="135a5-150">Request</span></span>

<span data-ttu-id="135a5-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="135a5-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="135a5-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="135a5-152">Response</span></span>

<span data-ttu-id="135a5-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="135a5-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="135a5-154">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="135a5-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```
