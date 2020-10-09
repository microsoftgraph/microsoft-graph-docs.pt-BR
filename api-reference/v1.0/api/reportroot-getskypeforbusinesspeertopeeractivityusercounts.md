---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: bd76bb21991ab3e1d0eb93409837dcedc3884f13
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401191"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="119c8-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="119c8-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

<span data-ttu-id="119c8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="119c8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="119c8-106">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="119c8-106">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="119c8-107">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="119c8-107">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="119c8-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Skype for Business peer-to-peer Activity](/skypeforbusiness/skype-for-business-online-reporting/peer-to-peer-activity-report).</span><span class="sxs-lookup"><span data-stu-id="119c8-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business peer-to-peer activity](/skypeforbusiness/skype-for-business-online-reporting/peer-to-peer-activity-report).</span></span>

## <a name="permissions"></a><span data-ttu-id="119c8-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="119c8-109">Permissions</span></span>

<span data-ttu-id="119c8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="119c8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="119c8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="119c8-112">Permission type</span></span>                        | <span data-ttu-id="119c8-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="119c8-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="119c8-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="119c8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="119c8-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="119c8-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="119c8-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="119c8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="119c8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="119c8-117">Not supported.</span></span>                           |
| <span data-ttu-id="119c8-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="119c8-118">Application</span></span>                            | <span data-ttu-id="119c8-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="119c8-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="119c8-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="119c8-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="119c8-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="119c8-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="119c8-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="119c8-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="119c8-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="119c8-123">Function parameters</span></span>

<span data-ttu-id="119c8-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="119c8-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="119c8-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="119c8-125">Parameter</span></span> | <span data-ttu-id="119c8-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="119c8-126">Type</span></span>   | <span data-ttu-id="119c8-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="119c8-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="119c8-128">ponto</span><span class="sxs-lookup"><span data-stu-id="119c8-128">period</span></span>    | <span data-ttu-id="119c8-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="119c8-129">string</span></span> | <span data-ttu-id="119c8-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="119c8-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="119c8-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="119c8-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="119c8-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="119c8-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="119c8-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="119c8-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="119c8-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="119c8-134">Request headers</span></span>

| <span data-ttu-id="119c8-135">Nome</span><span class="sxs-lookup"><span data-stu-id="119c8-135">Name</span></span>          | <span data-ttu-id="119c8-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="119c8-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="119c8-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="119c8-137">Authorization</span></span> | <span data-ttu-id="119c8-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="119c8-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="119c8-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="119c8-140">If-None-Match</span></span> | <span data-ttu-id="119c8-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="119c8-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="119c8-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="119c8-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="119c8-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="119c8-143">Response</span></span>

<span data-ttu-id="119c8-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="119c8-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="119c8-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="119c8-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="119c8-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="119c8-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="119c8-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="119c8-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="119c8-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="119c8-148">Report Refresh Date</span></span>
- <span data-ttu-id="119c8-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="119c8-149">Report Date</span></span>
- <span data-ttu-id="119c8-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="119c8-150">Report Period</span></span>
- <span data-ttu-id="119c8-151">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="119c8-151">IM</span></span>
- <span data-ttu-id="119c8-152">Áudio</span><span class="sxs-lookup"><span data-stu-id="119c8-152">Audio</span></span>
- <span data-ttu-id="119c8-153">Vídeo</span><span class="sxs-lookup"><span data-stu-id="119c8-153">Video</span></span>
- <span data-ttu-id="119c8-154">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="119c8-154">App Sharing</span></span>
- <span data-ttu-id="119c8-155">Transferência de arquivos</span><span class="sxs-lookup"><span data-stu-id="119c8-155">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="119c8-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="119c8-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="119c8-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="119c8-157">Request</span></span>

<span data-ttu-id="119c8-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="119c8-158">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="119c8-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="119c8-159">Response</span></span>

<span data-ttu-id="119c8-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="119c8-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="119c8-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="119c8-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
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