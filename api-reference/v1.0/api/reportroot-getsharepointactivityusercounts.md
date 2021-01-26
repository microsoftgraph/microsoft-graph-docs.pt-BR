---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 7a3cb1ef2e0fff5cfa61df6a3dd63f2baf6769b8
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980651"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="624f7-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="624f7-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="624f7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="624f7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="624f7-106">Obtenha a tendência no número de usuários ativos.</span><span class="sxs-lookup"><span data-stu-id="624f7-106">Get the trend in the number of active users.</span></span> <span data-ttu-id="624f7-107">Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="624f7-107">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="624f7-108">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte [relatórios do Microsoft 365 - Atividade do SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)</span><span class="sxs-lookup"><span data-stu-id="624f7-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="624f7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="624f7-109">Permissions</span></span>

<span data-ttu-id="624f7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="624f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="624f7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="624f7-112">Permission type</span></span>                        | <span data-ttu-id="624f7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="624f7-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="624f7-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="624f7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="624f7-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="624f7-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="624f7-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="624f7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="624f7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="624f7-117">Not supported.</span></span>                           |
| <span data-ttu-id="624f7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="624f7-118">Application</span></span>                            | <span data-ttu-id="624f7-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="624f7-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="624f7-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="624f7-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="624f7-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="624f7-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="624f7-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="624f7-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="624f7-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="624f7-123">Function parameters</span></span>

<span data-ttu-id="624f7-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="624f7-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="624f7-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="624f7-125">Parameter</span></span> | <span data-ttu-id="624f7-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="624f7-126">Type</span></span>   | <span data-ttu-id="624f7-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="624f7-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="624f7-128">ponto</span><span class="sxs-lookup"><span data-stu-id="624f7-128">period</span></span>    | <span data-ttu-id="624f7-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="624f7-129">string</span></span> | <span data-ttu-id="624f7-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="624f7-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="624f7-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="624f7-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="624f7-132">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="624f7-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="624f7-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="624f7-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="624f7-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="624f7-134">Request headers</span></span>

| <span data-ttu-id="624f7-135">Nome</span><span class="sxs-lookup"><span data-stu-id="624f7-135">Name</span></span>          | <span data-ttu-id="624f7-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="624f7-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="624f7-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="624f7-137">Authorization</span></span> | <span data-ttu-id="624f7-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="624f7-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="624f7-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="624f7-140">If-None-Match</span></span> | <span data-ttu-id="624f7-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="624f7-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="624f7-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="624f7-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="624f7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="624f7-143">Response</span></span>

<span data-ttu-id="624f7-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="624f7-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="624f7-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="624f7-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="624f7-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="624f7-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="624f7-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="624f7-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="624f7-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="624f7-148">Report Refresh Date</span></span>
- <span data-ttu-id="624f7-149">Página visitada</span><span class="sxs-lookup"><span data-stu-id="624f7-149">Visited Page</span></span>
- <span data-ttu-id="624f7-150">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="624f7-150">Viewed Or Edited</span></span>
- <span data-ttu-id="624f7-151">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="624f7-151">Synced</span></span>
- <span data-ttu-id="624f7-152">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="624f7-152">Shared Internally</span></span>
- <span data-ttu-id="624f7-153">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="624f7-153">Shared Externally</span></span>
- <span data-ttu-id="624f7-154">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="624f7-154">Report Date</span></span>
- <span data-ttu-id="624f7-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="624f7-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="624f7-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="624f7-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="624f7-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="624f7-157">Request</span></span>

<span data-ttu-id="624f7-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="624f7-158">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="624f7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="624f7-159">Response</span></span>

<span data-ttu-id="624f7-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="624f7-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="624f7-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="624f7-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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

