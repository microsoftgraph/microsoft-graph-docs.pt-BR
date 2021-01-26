---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts'
description: Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 62cf8cd8de20f3a6f9cf47241fadd677efa2f67f
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981393"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityminutecounts"></a><span data-ttu-id="5da74-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="5da74-104">reportRoot: getSkypeForBusinessOrganizerActivityMinuteCounts</span></span>

<span data-ttu-id="5da74-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5da74-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5da74-106">Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="5da74-106">Get usage trends on the length in minutes and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="5da74-107">Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5da74-107">Types of conference sessions include audio/video, and dial-in and dial-out - Microsoft.</span></span>

> <span data-ttu-id="5da74-108">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - atividade do organizador de conferências do Skype for Business.](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)</span><span class="sxs-lookup"><span data-stu-id="5da74-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="5da74-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5da74-109">Permissions</span></span>

<span data-ttu-id="5da74-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5da74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5da74-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5da74-112">Permission type</span></span>                        | <span data-ttu-id="5da74-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5da74-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5da74-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5da74-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5da74-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da74-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5da74-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5da74-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5da74-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5da74-117">Not supported.</span></span>                           |
| <span data-ttu-id="5da74-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5da74-118">Application</span></span>                            | <span data-ttu-id="5da74-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5da74-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="5da74-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="5da74-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5da74-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5da74-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5da74-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5da74-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5da74-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5da74-123">Function parameters</span></span>

<span data-ttu-id="5da74-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5da74-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5da74-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5da74-125">Parameter</span></span> | <span data-ttu-id="5da74-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="5da74-126">Type</span></span>   | <span data-ttu-id="5da74-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="5da74-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5da74-128">ponto</span><span class="sxs-lookup"><span data-stu-id="5da74-128">period</span></span>    | <span data-ttu-id="5da74-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5da74-129">string</span></span> | <span data-ttu-id="5da74-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5da74-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5da74-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5da74-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5da74-132">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5da74-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5da74-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5da74-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5da74-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5da74-134">Request headers</span></span>

| <span data-ttu-id="5da74-135">Nome</span><span class="sxs-lookup"><span data-stu-id="5da74-135">Name</span></span>          | <span data-ttu-id="5da74-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="5da74-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5da74-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="5da74-137">Authorization</span></span> | <span data-ttu-id="5da74-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5da74-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5da74-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5da74-140">If-None-Match</span></span> | <span data-ttu-id="5da74-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="5da74-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5da74-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5da74-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5da74-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5da74-143">Response</span></span>

<span data-ttu-id="5da74-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5da74-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5da74-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5da74-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5da74-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5da74-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5da74-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5da74-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5da74-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5da74-148">Report Refresh Date</span></span>
- <span data-ttu-id="5da74-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="5da74-149">Report Date</span></span>
- <span data-ttu-id="5da74-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5da74-150">Report Period</span></span>
- <span data-ttu-id="5da74-151">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="5da74-151">Audio/Video</span></span>
- <span data-ttu-id="5da74-152">Dial-in pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="5da74-152">Dial-in Microsoft</span></span>
- <span data-ttu-id="5da74-153">Dial-out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="5da74-153">Dial-out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="5da74-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5da74-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5da74-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5da74-155">Request</span></span>

<span data-ttu-id="5da74-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5da74-156">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="5da74-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="5da74-157">Response</span></span>

<span data-ttu-id="5da74-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5da74-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="5da74-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5da74-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video,Dial-in Microsoft,Dial-out Microsoft
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

