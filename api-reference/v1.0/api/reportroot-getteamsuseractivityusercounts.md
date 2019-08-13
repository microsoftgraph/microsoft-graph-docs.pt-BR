---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8c32bf9712be627933af96eb2c104260546cd210
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320419"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="ff8a0-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="ff8a0-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="ff8a0-105">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="ff8a0-106">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff8a0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff8a0-107">Permissions</span></span>

<span data-ttu-id="ff8a0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff8a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff8a0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff8a0-110">Permission type</span></span>                        | <span data-ttu-id="ff8a0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff8a0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ff8a0-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff8a0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff8a0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff8a0-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ff8a0-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff8a0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff8a0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-115">Not supported.</span></span>                           |
| <span data-ttu-id="ff8a0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff8a0-116">Application</span></span>                            | <span data-ttu-id="ff8a0-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff8a0-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ff8a0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff8a0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ff8a0-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ff8a0-119">Function parameters</span></span>

<span data-ttu-id="ff8a0-120">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ff8a0-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ff8a0-121">Parameter</span></span> | <span data-ttu-id="ff8a0-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff8a0-122">Type</span></span>   | <span data-ttu-id="ff8a0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff8a0-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ff8a0-124">ponto</span><span class="sxs-lookup"><span data-stu-id="ff8a0-124">period</span></span>    | <span data-ttu-id="ff8a0-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff8a0-125">string</span></span> | <span data-ttu-id="ff8a0-126">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ff8a0-127">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ff8a0-128">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ff8a0-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ff8a0-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff8a0-130">Request headers</span></span>

| <span data-ttu-id="ff8a0-131">Nome</span><span class="sxs-lookup"><span data-stu-id="ff8a0-131">Name</span></span>          | <span data-ttu-id="ff8a0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff8a0-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ff8a0-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff8a0-133">Authorization</span></span> | <span data-ttu-id="ff8a0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ff8a0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff8a0-136">Response</span></span>

<span data-ttu-id="ff8a0-137">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ff8a0-138">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ff8a0-139">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ff8a0-140">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="ff8a0-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="ff8a0-141">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ff8a0-141">Report Refresh Date</span></span>
- <span data-ttu-id="ff8a0-142">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="ff8a0-142">Report Date</span></span>
- <span data-ttu-id="ff8a0-143">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="ff8a0-143">Team Chat Messages</span></span>
- <span data-ttu-id="ff8a0-144">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="ff8a0-144">Private Chat Messages</span></span>
- <span data-ttu-id="ff8a0-145">Chamadas</span><span class="sxs-lookup"><span data-stu-id="ff8a0-145">Calls</span></span>
- <span data-ttu-id="ff8a0-146">Reuniões</span><span class="sxs-lookup"><span data-stu-id="ff8a0-146">Meetings</span></span>
- <span data-ttu-id="ff8a0-147">Outras Ações</span><span class="sxs-lookup"><span data-stu-id="ff8a0-147">Other Actions</span></span>
- <span data-ttu-id="ff8a0-148">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ff8a0-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ff8a0-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff8a0-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ff8a0-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff8a0-150">Request</span></span>

<span data-ttu-id="ff8a0-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-151">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ff8a0-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff8a0-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff8a0-153">C#</span><span class="sxs-lookup"><span data-stu-id="ff8a0-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff8a0-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff8a0-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff8a0-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ff8a0-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff8a0-156">Java</span><span class="sxs-lookup"><span data-stu-id="ff8a0-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ff8a0-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff8a0-157">Response</span></span>

<span data-ttu-id="ff8a0-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="ff8a0-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ff8a0-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
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
