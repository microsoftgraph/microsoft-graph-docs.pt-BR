---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e138c8960fbae32b5af95fb8743633e206d47697
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589135"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="21d3f-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="21d3f-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="21d3f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21d3f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="21d3f-106">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="21d3f-106">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="21d3f-107">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="21d3f-107">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="21d3f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="21d3f-108">Permissions</span></span>

<span data-ttu-id="21d3f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21d3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21d3f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21d3f-111">Permission type</span></span>                        | <span data-ttu-id="21d3f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21d3f-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="21d3f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21d3f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="21d3f-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="21d3f-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="21d3f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21d3f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21d3f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21d3f-116">Not supported.</span></span>                           |
| <span data-ttu-id="21d3f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21d3f-117">Application</span></span>                            | <span data-ttu-id="21d3f-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="21d3f-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="21d3f-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="21d3f-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="21d3f-120">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="21d3f-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="21d3f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21d3f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="21d3f-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="21d3f-122">Function parameters</span></span>

<span data-ttu-id="21d3f-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="21d3f-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="21d3f-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="21d3f-124">Parameter</span></span> | <span data-ttu-id="21d3f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="21d3f-125">Type</span></span>   | <span data-ttu-id="21d3f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="21d3f-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="21d3f-127">ponto</span><span class="sxs-lookup"><span data-stu-id="21d3f-127">period</span></span>    | <span data-ttu-id="21d3f-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21d3f-128">string</span></span> | <span data-ttu-id="21d3f-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="21d3f-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="21d3f-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="21d3f-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="21d3f-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="21d3f-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="21d3f-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21d3f-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="21d3f-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21d3f-133">Request headers</span></span>

| <span data-ttu-id="21d3f-134">Nome</span><span class="sxs-lookup"><span data-stu-id="21d3f-134">Name</span></span>          | <span data-ttu-id="21d3f-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="21d3f-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="21d3f-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="21d3f-136">Authorization</span></span> | <span data-ttu-id="21d3f-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21d3f-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="21d3f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="21d3f-139">Response</span></span>

<span data-ttu-id="21d3f-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="21d3f-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="21d3f-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="21d3f-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="21d3f-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="21d3f-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="21d3f-143">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="21d3f-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="21d3f-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="21d3f-144">Report Refresh Date</span></span>
- <span data-ttu-id="21d3f-145">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="21d3f-145">Report Date</span></span>
- <span data-ttu-id="21d3f-146">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="21d3f-146">Team Chat Messages</span></span>
- <span data-ttu-id="21d3f-147">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="21d3f-147">Private Chat Messages</span></span>
- <span data-ttu-id="21d3f-148">Chamadas</span><span class="sxs-lookup"><span data-stu-id="21d3f-148">Calls</span></span>
- <span data-ttu-id="21d3f-149">Reuniões</span><span class="sxs-lookup"><span data-stu-id="21d3f-149">Meetings</span></span>
- <span data-ttu-id="21d3f-150">Outras Ações</span><span class="sxs-lookup"><span data-stu-id="21d3f-150">Other Actions</span></span>
- <span data-ttu-id="21d3f-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="21d3f-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="21d3f-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21d3f-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="21d3f-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21d3f-153">Request</span></span>

<span data-ttu-id="21d3f-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="21d3f-154">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="21d3f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="21d3f-155">Response</span></span>

<span data-ttu-id="21d3f-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21d3f-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="21d3f-157">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="21d3f-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
