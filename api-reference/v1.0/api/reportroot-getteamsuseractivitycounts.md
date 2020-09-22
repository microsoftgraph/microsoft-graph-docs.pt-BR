---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e21fc78550d72e16c3931dbbe299e2a70aa908fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013045"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="ed620-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ed620-104">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="ed620-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed620-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed620-106">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="ed620-106">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="ed620-107">Os tipos de atividade são mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões.</span><span class="sxs-lookup"><span data-stu-id="ed620-107">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed620-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed620-108">Permissions</span></span>

<span data-ttu-id="ed620-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed620-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed620-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed620-111">Permission type</span></span>                        | <span data-ttu-id="ed620-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed620-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ed620-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed620-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed620-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed620-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ed620-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed620-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed620-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed620-116">Not supported.</span></span>                           |
| <span data-ttu-id="ed620-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed620-117">Application</span></span>                            | <span data-ttu-id="ed620-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed620-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="ed620-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="ed620-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ed620-120">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ed620-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ed620-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed620-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ed620-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ed620-122">Function parameters</span></span>

<span data-ttu-id="ed620-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ed620-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ed620-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ed620-124">Parameter</span></span> | <span data-ttu-id="ed620-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed620-125">Type</span></span>   | <span data-ttu-id="ed620-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed620-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ed620-127">ponto</span><span class="sxs-lookup"><span data-stu-id="ed620-127">period</span></span>    | <span data-ttu-id="ed620-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed620-128">string</span></span> | <span data-ttu-id="ed620-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ed620-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ed620-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ed620-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ed620-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ed620-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ed620-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed620-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ed620-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed620-133">Request headers</span></span>

| <span data-ttu-id="ed620-134">Nome</span><span class="sxs-lookup"><span data-stu-id="ed620-134">Name</span></span>          | <span data-ttu-id="ed620-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed620-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ed620-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed620-136">Authorization</span></span> | <span data-ttu-id="ed620-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed620-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ed620-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed620-139">Response</span></span>

<span data-ttu-id="ed620-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ed620-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ed620-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ed620-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ed620-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ed620-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ed620-143">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="ed620-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="ed620-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ed620-144">Report Refresh Date</span></span>
- <span data-ttu-id="ed620-145">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="ed620-145">Report Date</span></span>
- <span data-ttu-id="ed620-146">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="ed620-146">Team Chat Messages</span></span>
- <span data-ttu-id="ed620-147">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="ed620-147">Private Chat Messages</span></span>
- <span data-ttu-id="ed620-148">Chamadas</span><span class="sxs-lookup"><span data-stu-id="ed620-148">Calls</span></span>
- <span data-ttu-id="ed620-149">Reuniões</span><span class="sxs-lookup"><span data-stu-id="ed620-149">Meetings</span></span>
- <span data-ttu-id="ed620-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ed620-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ed620-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed620-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ed620-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed620-152">Request</span></span>

<span data-ttu-id="ed620-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed620-153">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="ed620-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed620-154">Response</span></span>

<span data-ttu-id="ed620-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ed620-155">The following is an example of the response.</span></span>

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
<span data-ttu-id="ed620-156">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ed620-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
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

