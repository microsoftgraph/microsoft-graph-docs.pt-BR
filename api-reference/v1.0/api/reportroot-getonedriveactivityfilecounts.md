---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 7f03aa980ceead767ea59f641620c212dbbfabb5
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983010"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a><span data-ttu-id="94c1c-103">reportRoot: getOneDriveActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="94c1c-103">reportRoot: getOneDriveActivityFileCounts</span></span>

<span data-ttu-id="94c1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94c1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94c1c-105">Obtenha o número de usuários únicos licenciados que realizaram interações de arquivos contra qualquer conta do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="94c1c-105">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span>

> <span data-ttu-id="94c1c-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, confira [relatórios do Microsoft 365 - atividade do OneDrive for Business.](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)</span><span class="sxs-lookup"><span data-stu-id="94c1c-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="94c1c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="94c1c-107">Permissions</span></span>

<span data-ttu-id="94c1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94c1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94c1c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94c1c-110">Permission type</span></span>                        | <span data-ttu-id="94c1c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94c1c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="94c1c-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94c1c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="94c1c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="94c1c-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="94c1c-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94c1c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94c1c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94c1c-115">Not supported.</span></span>                           |
| <span data-ttu-id="94c1c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94c1c-116">Application</span></span>                            | <span data-ttu-id="94c1c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="94c1c-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="94c1c-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="94c1c-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="94c1c-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="94c1c-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="94c1c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94c1c-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="94c1c-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="94c1c-121">Function parameters</span></span>

<span data-ttu-id="94c1c-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="94c1c-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="94c1c-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="94c1c-123">Parameter</span></span> | <span data-ttu-id="94c1c-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="94c1c-124">Type</span></span>   | <span data-ttu-id="94c1c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="94c1c-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="94c1c-126">ponto</span><span class="sxs-lookup"><span data-stu-id="94c1c-126">period</span></span>    | <span data-ttu-id="94c1c-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94c1c-127">string</span></span> | <span data-ttu-id="94c1c-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="94c1c-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="94c1c-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="94c1c-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="94c1c-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="94c1c-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="94c1c-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94c1c-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="94c1c-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94c1c-132">Request headers</span></span>

| <span data-ttu-id="94c1c-133">Nome</span><span class="sxs-lookup"><span data-stu-id="94c1c-133">Name</span></span>          | <span data-ttu-id="94c1c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="94c1c-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="94c1c-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="94c1c-135">Authorization</span></span> | <span data-ttu-id="94c1c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94c1c-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="94c1c-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="94c1c-138">If-None-Match</span></span> | <span data-ttu-id="94c1c-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="94c1c-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="94c1c-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="94c1c-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="94c1c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="94c1c-141">Response</span></span>

<span data-ttu-id="94c1c-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="94c1c-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="94c1c-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="94c1c-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="94c1c-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="94c1c-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="94c1c-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="94c1c-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="94c1c-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="94c1c-146">Report Refresh Date</span></span>
- <span data-ttu-id="94c1c-147">Exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="94c1c-147">Viewed Or Edited</span></span>
- <span data-ttu-id="94c1c-148">Sincronizados</span><span class="sxs-lookup"><span data-stu-id="94c1c-148">Synced</span></span>
- <span data-ttu-id="94c1c-149">Compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="94c1c-149">Shared Internally</span></span>
- <span data-ttu-id="94c1c-150">Compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="94c1c-150">Shared Externally</span></span>
- <span data-ttu-id="94c1c-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="94c1c-151">Report Date</span></span>
- <span data-ttu-id="94c1c-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="94c1c-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="94c1c-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94c1c-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="94c1c-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94c1c-154">Request</span></span>

<span data-ttu-id="94c1c-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94c1c-155">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityfilecounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityFileCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="94c1c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="94c1c-156">Response</span></span>

<span data-ttu-id="94c1c-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94c1c-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="94c1c-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="94c1c-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
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

