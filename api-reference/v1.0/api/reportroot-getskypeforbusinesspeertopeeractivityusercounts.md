---
title: 'reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts'
description: Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 65fa7bdc5f15d348368982096b31f5a3dfacc917
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864233"
---
# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="83021-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="83021-104">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

<span data-ttu-id="83021-105">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização.</span><span class="sxs-lookup"><span data-stu-id="83021-105">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="83021-106">Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="83021-106">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="83021-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://docs.microsoft.com/skypeforbusiness/skype-for-business-online-reporting/peer-to-peer-activity-report).</span><span class="sxs-lookup"><span data-stu-id="83021-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://docs.microsoft.com/skypeforbusiness/skype-for-business-online-reporting/peer-to-peer-activity-report).</span></span>

## <a name="permissions"></a><span data-ttu-id="83021-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="83021-108">Permissions</span></span>

<span data-ttu-id="83021-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83021-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83021-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83021-111">Permission type</span></span>                        | <span data-ttu-id="83021-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83021-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="83021-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83021-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="83021-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83021-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="83021-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83021-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83021-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83021-116">Not supported.</span></span>                           |
| <span data-ttu-id="83021-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83021-117">Application</span></span>                            | <span data-ttu-id="83021-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83021-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="83021-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="83021-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="83021-120">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="83021-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="83021-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83021-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="83021-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="83021-122">Function parameters</span></span>

<span data-ttu-id="83021-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="83021-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="83021-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="83021-124">Parameter</span></span> | <span data-ttu-id="83021-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="83021-125">Type</span></span>   | <span data-ttu-id="83021-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="83021-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="83021-127">ponto</span><span class="sxs-lookup"><span data-stu-id="83021-127">period</span></span>    | <span data-ttu-id="83021-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83021-128">string</span></span> | <span data-ttu-id="83021-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="83021-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="83021-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="83021-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="83021-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="83021-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="83021-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83021-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="83021-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83021-133">Request headers</span></span>

| <span data-ttu-id="83021-134">Nome</span><span class="sxs-lookup"><span data-stu-id="83021-134">Name</span></span>          | <span data-ttu-id="83021-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="83021-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="83021-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="83021-136">Authorization</span></span> | <span data-ttu-id="83021-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83021-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="83021-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="83021-139">If-None-Match</span></span> | <span data-ttu-id="83021-140">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="83021-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="83021-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="83021-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="83021-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="83021-142">Response</span></span>

<span data-ttu-id="83021-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="83021-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="83021-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="83021-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="83021-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="83021-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="83021-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="83021-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="83021-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="83021-147">Report Refresh Date</span></span>
- <span data-ttu-id="83021-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="83021-148">Report Date</span></span>
- <span data-ttu-id="83021-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="83021-149">Report Period</span></span>
- <span data-ttu-id="83021-150">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="83021-150">IM</span></span>
- <span data-ttu-id="83021-151">Áudio</span><span class="sxs-lookup"><span data-stu-id="83021-151">Audio</span></span>
- <span data-ttu-id="83021-152">Vídeo</span><span class="sxs-lookup"><span data-stu-id="83021-152">Video</span></span>
- <span data-ttu-id="83021-153">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="83021-153">App Sharing</span></span>
- <span data-ttu-id="83021-154">Transferência de arquivos</span><span class="sxs-lookup"><span data-stu-id="83021-154">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="83021-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83021-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="83021-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83021-156">Request</span></span>

<span data-ttu-id="83021-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83021-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="83021-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="83021-158">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="83021-159">C#</span><span class="sxs-lookup"><span data-stu-id="83021-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinesspeertopeeractivityusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83021-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83021-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinesspeertopeeractivityusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="83021-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83021-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinesspeertopeeractivityusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="83021-162">Java</span><span class="sxs-lookup"><span data-stu-id="83021-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinesspeertopeeractivityusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="83021-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="83021-163">Response</span></span>

<span data-ttu-id="83021-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83021-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="83021-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="83021-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
