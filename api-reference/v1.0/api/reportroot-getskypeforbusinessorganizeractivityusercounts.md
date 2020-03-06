---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 5f491951000b28ef028bca9a89f332e5aaeaca77
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510127"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="ad5e8-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="ad5e8-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

<span data-ttu-id="ad5e8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad5e8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad5e8-106">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-106">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="ad5e8-107">Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-107">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="ad5e8-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do organizador da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="ad5e8-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad5e8-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad5e8-109">Permissions</span></span>

<span data-ttu-id="ad5e8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad5e8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad5e8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad5e8-112">Permission type</span></span>                        | <span data-ttu-id="ad5e8-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad5e8-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ad5e8-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad5e8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad5e8-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad5e8-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ad5e8-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad5e8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad5e8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-117">Not supported.</span></span>                           |
| <span data-ttu-id="ad5e8-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad5e8-118">Application</span></span>                            | <span data-ttu-id="ad5e8-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad5e8-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="ad5e8-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ad5e8-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ad5e8-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ad5e8-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad5e8-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ad5e8-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ad5e8-123">Function parameters</span></span>

<span data-ttu-id="ad5e8-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ad5e8-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ad5e8-125">Parameter</span></span> | <span data-ttu-id="ad5e8-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad5e8-126">Type</span></span>   | <span data-ttu-id="ad5e8-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad5e8-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ad5e8-128">ponto</span><span class="sxs-lookup"><span data-stu-id="ad5e8-128">period</span></span>    | <span data-ttu-id="ad5e8-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad5e8-129">string</span></span> | <span data-ttu-id="ad5e8-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ad5e8-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ad5e8-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ad5e8-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ad5e8-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad5e8-134">Request headers</span></span>

| <span data-ttu-id="ad5e8-135">Nome</span><span class="sxs-lookup"><span data-stu-id="ad5e8-135">Name</span></span>          | <span data-ttu-id="ad5e8-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad5e8-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ad5e8-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad5e8-137">Authorization</span></span> | <span data-ttu-id="ad5e8-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ad5e8-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ad5e8-140">If-None-Match</span></span> | <span data-ttu-id="ad5e8-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ad5e8-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ad5e8-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad5e8-143">Response</span></span>

<span data-ttu-id="ad5e8-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ad5e8-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ad5e8-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ad5e8-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ad5e8-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ad5e8-148">Report Refresh Date</span></span>
- <span data-ttu-id="ad5e8-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="ad5e8-149">Report Date</span></span>
- <span data-ttu-id="ad5e8-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ad5e8-150">Report Period</span></span>
- <span data-ttu-id="ad5e8-151">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="ad5e8-151">IM</span></span>
- <span data-ttu-id="ad5e8-152">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="ad5e8-152">Audio/Video</span></span>
- <span data-ttu-id="ad5e8-153">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="ad5e8-153">App Sharing</span></span>
- <span data-ttu-id="ad5e8-154">Web</span><span class="sxs-lookup"><span data-stu-id="ad5e8-154">Web</span></span>
- <span data-ttu-id="ad5e8-155">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="ad5e8-155">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="ad5e8-156">Dial-in/out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="ad5e8-156">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="ad5e8-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad5e8-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ad5e8-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad5e8-158">Request</span></span>

<span data-ttu-id="ad5e8-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad5e8-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad5e8-160">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="ad5e8-161">C#</span><span class="sxs-lookup"><span data-stu-id="ad5e8-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad5e8-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad5e8-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad5e8-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad5e8-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad5e8-164">Java</span><span class="sxs-lookup"><span data-stu-id="ad5e8-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ad5e8-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad5e8-165">Response</span></span>

<span data-ttu-id="ad5e8-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="ad5e8-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ad5e8-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
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
