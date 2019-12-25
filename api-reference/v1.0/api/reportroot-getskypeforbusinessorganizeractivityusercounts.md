---
title: 'reportRoot: getSkypeForBusinessOrganizerActivityUserCounts'
description: Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 84a50cab95f9ec2b7f8e8380815fdc27ca6547f1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865286"
---
# <a name="reportroot-getskypeforbusinessorganizeractivityusercounts"></a><span data-ttu-id="6c1cd-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="6c1cd-104">reportRoot: getSkypeForBusinessOrganizerActivityUserCounts</span></span>

<span data-ttu-id="6c1cd-105">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-105">Get usage trends on the number of unique users and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="6c1cd-106">Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-106">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and dial-in/out Microsoft.</span></span>

> <span data-ttu-id="6c1cd-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do organizador da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="6c1cd-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="6c1cd-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c1cd-108">Permissions</span></span>

<span data-ttu-id="6c1cd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c1cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c1cd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c1cd-111">Permission type</span></span>                        | <span data-ttu-id="6c1cd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c1cd-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6c1cd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c1cd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c1cd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c1cd-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6c1cd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c1cd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c1cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-116">Not supported.</span></span>                           |
| <span data-ttu-id="6c1cd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c1cd-117">Application</span></span>                            | <span data-ttu-id="6c1cd-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c1cd-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="6c1cd-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="6c1cd-120">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="6c1cd-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="6c1cd-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c1cd-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6c1cd-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="6c1cd-122">Function parameters</span></span>

<span data-ttu-id="6c1cd-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6c1cd-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6c1cd-124">Parameter</span></span> | <span data-ttu-id="6c1cd-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c1cd-125">Type</span></span>   | <span data-ttu-id="6c1cd-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c1cd-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6c1cd-127">ponto</span><span class="sxs-lookup"><span data-stu-id="6c1cd-127">period</span></span>    | <span data-ttu-id="6c1cd-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c1cd-128">string</span></span> | <span data-ttu-id="6c1cd-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6c1cd-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6c1cd-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6c1cd-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6c1cd-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c1cd-133">Request headers</span></span>

| <span data-ttu-id="6c1cd-134">Nome</span><span class="sxs-lookup"><span data-stu-id="6c1cd-134">Name</span></span>          | <span data-ttu-id="6c1cd-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c1cd-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6c1cd-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c1cd-136">Authorization</span></span> | <span data-ttu-id="6c1cd-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6c1cd-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6c1cd-139">If-None-Match</span></span> | <span data-ttu-id="6c1cd-140">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6c1cd-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6c1cd-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c1cd-142">Response</span></span>

<span data-ttu-id="6c1cd-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6c1cd-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6c1cd-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6c1cd-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6c1cd-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="6c1cd-147">Report Refresh Date</span></span>
- <span data-ttu-id="6c1cd-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="6c1cd-148">Report Date</span></span>
- <span data-ttu-id="6c1cd-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="6c1cd-149">Report Period</span></span>
- <span data-ttu-id="6c1cd-150">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="6c1cd-150">IM</span></span>
- <span data-ttu-id="6c1cd-151">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="6c1cd-151">Audio/Video</span></span>
- <span data-ttu-id="6c1cd-152">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="6c1cd-152">App Sharing</span></span>
- <span data-ttu-id="6c1cd-153">Web</span><span class="sxs-lookup"><span data-stu-id="6c1cd-153">Web</span></span>
- <span data-ttu-id="6c1cd-154">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="6c1cd-154">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="6c1cd-155">Dial-in/out pela Microsoft</span><span class="sxs-lookup"><span data-stu-id="6c1cd-155">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="6c1cd-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c1cd-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6c1cd-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c1cd-157">Request</span></span>

<span data-ttu-id="6c1cd-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6c1cd-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c1cd-159">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6c1cd-160">C#</span><span class="sxs-lookup"><span data-stu-id="6c1cd-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessorganizeractivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c1cd-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c1cd-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessorganizeractivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6c1cd-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c1cd-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessorganizeractivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6c1cd-163">Java</span><span class="sxs-lookup"><span data-stu-id="6c1cd-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessorganizeractivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6c1cd-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c1cd-164">Response</span></span>

<span data-ttu-id="6c1cd-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="6c1cd-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="6c1cd-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
