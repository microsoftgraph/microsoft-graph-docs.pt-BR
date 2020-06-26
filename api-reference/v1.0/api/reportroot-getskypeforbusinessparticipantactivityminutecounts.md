---
title: 'reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts'
description: Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem áudio/vídeo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 183a9e201bfe397af6b3c307a355134cbf132554
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44892416"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="364c7-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="364c7-104">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="364c7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="364c7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="364c7-106">Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="364c7-106">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="364c7-107">Tipos de sessões de conferência incluem áudio/vídeo.</span><span class="sxs-lookup"><span data-stu-id="364c7-107">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="364c7-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Skype for Business Conference participante Activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="364c7-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="364c7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="364c7-109">Permissions</span></span>

<span data-ttu-id="364c7-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="364c7-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="364c7-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="364c7-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="364c7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="364c7-112">Permission type</span></span>                        | <span data-ttu-id="364c7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="364c7-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="364c7-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="364c7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="364c7-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="364c7-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="364c7-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="364c7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="364c7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="364c7-117">Not supported.</span></span>                           |
| <span data-ttu-id="364c7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="364c7-118">Application</span></span>                            | <span data-ttu-id="364c7-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="364c7-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="364c7-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="364c7-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="364c7-121">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="364c7-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="364c7-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="364c7-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="364c7-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="364c7-123">Function parameters</span></span>

<span data-ttu-id="364c7-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="364c7-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="364c7-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="364c7-125">Parameter</span></span> | <span data-ttu-id="364c7-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="364c7-126">Type</span></span>   | <span data-ttu-id="364c7-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="364c7-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="364c7-128">ponto</span><span class="sxs-lookup"><span data-stu-id="364c7-128">period</span></span>    | <span data-ttu-id="364c7-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="364c7-129">string</span></span> | <span data-ttu-id="364c7-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="364c7-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="364c7-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="364c7-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="364c7-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="364c7-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="364c7-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="364c7-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="364c7-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="364c7-134">Request headers</span></span>

| <span data-ttu-id="364c7-135">Nome</span><span class="sxs-lookup"><span data-stu-id="364c7-135">Name</span></span>          | <span data-ttu-id="364c7-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="364c7-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="364c7-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="364c7-137">Authorization</span></span> | <span data-ttu-id="364c7-138">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="364c7-138">Bearer {token}.</span></span> <span data-ttu-id="364c7-139">Required.</span><span class="sxs-lookup"><span data-stu-id="364c7-139">Required.</span></span>                |
| <span data-ttu-id="364c7-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="364c7-140">If-None-Match</span></span> | <span data-ttu-id="364c7-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="364c7-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="364c7-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="364c7-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="364c7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="364c7-143">Response</span></span>

<span data-ttu-id="364c7-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="364c7-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="364c7-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="364c7-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="364c7-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="364c7-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="364c7-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="364c7-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="364c7-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="364c7-148">Report Refresh Date</span></span>
- <span data-ttu-id="364c7-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="364c7-149">Report Date</span></span>
- <span data-ttu-id="364c7-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="364c7-150">Report Period</span></span>
- <span data-ttu-id="364c7-151">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="364c7-151">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="364c7-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="364c7-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="364c7-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="364c7-153">Request</span></span>

<span data-ttu-id="364c7-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="364c7-154">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="364c7-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="364c7-155">Response</span></span>

<span data-ttu-id="364c7-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="364c7-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="364c7-157">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="364c7-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
