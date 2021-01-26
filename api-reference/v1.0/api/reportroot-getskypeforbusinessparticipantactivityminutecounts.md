---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem áudio/vídeo.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: ac9924c04fd069a3defe76cc100fe80344f70c57
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981204"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="b9a87-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="b9a87-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="b9a87-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9a87-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9a87-106">Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="b9a87-106">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="b9a87-107">Tipos de sessões de conferência incluem áudio/vídeo.</span><span class="sxs-lookup"><span data-stu-id="b9a87-107">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="b9a87-108">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - Atividade de participantes de conferências do Skype for Business.](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)</span><span class="sxs-lookup"><span data-stu-id="b9a87-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9a87-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9a87-109">Permissions</span></span>

<span data-ttu-id="b9a87-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9a87-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9a87-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9a87-112">Permission type</span></span>                        | <span data-ttu-id="b9a87-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9a87-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b9a87-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9a87-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9a87-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9a87-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b9a87-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9a87-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9a87-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9a87-117">Not supported.</span></span>                           |
| <span data-ttu-id="b9a87-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9a87-118">Application</span></span>                            | <span data-ttu-id="b9a87-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9a87-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="b9a87-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="b9a87-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="b9a87-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="b9a87-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="b9a87-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9a87-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b9a87-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b9a87-123">Function parameters</span></span>

<span data-ttu-id="b9a87-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b9a87-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b9a87-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9a87-125">Parameter</span></span> | <span data-ttu-id="b9a87-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9a87-126">Type</span></span>   | <span data-ttu-id="b9a87-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9a87-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b9a87-128">ponto</span><span class="sxs-lookup"><span data-stu-id="b9a87-128">period</span></span>    | <span data-ttu-id="b9a87-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9a87-129">string</span></span> | <span data-ttu-id="b9a87-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b9a87-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b9a87-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b9a87-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b9a87-132">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b9a87-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b9a87-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9a87-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b9a87-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a87-134">Request headers</span></span>

| <span data-ttu-id="b9a87-135">Nome</span><span class="sxs-lookup"><span data-stu-id="b9a87-135">Name</span></span>          | <span data-ttu-id="b9a87-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9a87-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b9a87-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9a87-137">Authorization</span></span> | <span data-ttu-id="b9a87-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9a87-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b9a87-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b9a87-140">If-None-Match</span></span> | <span data-ttu-id="b9a87-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="b9a87-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b9a87-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b9a87-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b9a87-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a87-143">Response</span></span>

<span data-ttu-id="b9a87-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b9a87-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b9a87-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b9a87-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b9a87-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b9a87-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b9a87-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b9a87-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b9a87-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b9a87-148">Report Refresh Date</span></span>
- <span data-ttu-id="b9a87-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="b9a87-149">Report Date</span></span>
- <span data-ttu-id="b9a87-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b9a87-150">Report Period</span></span>
- <span data-ttu-id="b9a87-151">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="b9a87-151">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="b9a87-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9a87-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b9a87-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a87-153">Request</span></span>

<span data-ttu-id="b9a87-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9a87-154">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="b9a87-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a87-155">Response</span></span>

<span data-ttu-id="b9a87-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b9a87-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="b9a87-157">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b9a87-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
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

