---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Obtenha a contagem de usuários ativos diários no período de relatório por produto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f5e49018ddc6d0f576fffbd03b39d69675475eee
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865409"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="9b04d-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="9b04d-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="9b04d-104">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="9b04d-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="9b04d-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="9b04d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b04d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b04d-106">Permissions</span></span>

<span data-ttu-id="9b04d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b04d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b04d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b04d-109">Permission type</span></span>                        | <span data-ttu-id="9b04d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b04d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9b04d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b04d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b04d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b04d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9b04d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b04d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b04d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b04d-114">Not supported.</span></span>                           |
| <span data-ttu-id="9b04d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b04d-115">Application</span></span>                            | <span data-ttu-id="9b04d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b04d-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="9b04d-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="9b04d-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="9b04d-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="9b04d-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="9b04d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b04d-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9b04d-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9b04d-120">Function parameters</span></span>

<span data-ttu-id="9b04d-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="9b04d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9b04d-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9b04d-122">Parameter</span></span> | <span data-ttu-id="9b04d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b04d-123">Type</span></span>   | <span data-ttu-id="9b04d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b04d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9b04d-125">ponto</span><span class="sxs-lookup"><span data-stu-id="9b04d-125">period</span></span>    | <span data-ttu-id="9b04d-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b04d-126">string</span></span> | <span data-ttu-id="9b04d-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9b04d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9b04d-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="9b04d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9b04d-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="9b04d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9b04d-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b04d-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9b04d-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b04d-131">Request headers</span></span>

| <span data-ttu-id="9b04d-132">Nome</span><span class="sxs-lookup"><span data-stu-id="9b04d-132">Name</span></span>          | <span data-ttu-id="9b04d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b04d-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9b04d-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b04d-134">Authorization</span></span> | <span data-ttu-id="9b04d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b04d-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9b04d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b04d-137">Response</span></span>

<span data-ttu-id="9b04d-138">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="9b04d-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9b04d-139">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="9b04d-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9b04d-140">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9b04d-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9b04d-141">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="9b04d-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9b04d-142">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="9b04d-142">Report Refresh Date</span></span>
- <span data-ttu-id="9b04d-143">Office 365</span><span class="sxs-lookup"><span data-stu-id="9b04d-143">Office 365</span></span>
- <span data-ttu-id="9b04d-144">Exchange</span><span class="sxs-lookup"><span data-stu-id="9b04d-144">Exchange</span></span>
- <span data-ttu-id="9b04d-145">OneDrive</span><span class="sxs-lookup"><span data-stu-id="9b04d-145">OneDrive</span></span>
- <span data-ttu-id="9b04d-146">SharePoint</span><span class="sxs-lookup"><span data-stu-id="9b04d-146">SharePoint</span></span>
- <span data-ttu-id="9b04d-147">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="9b04d-147">Skype For Business</span></span> 
- <span data-ttu-id="9b04d-148">Yammer</span><span class="sxs-lookup"><span data-stu-id="9b04d-148">Yammer</span></span>
- <span data-ttu-id="9b04d-149">Teams</span><span class="sxs-lookup"><span data-stu-id="9b04d-149">Teams</span></span>
- <span data-ttu-id="9b04d-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="9b04d-150">Report Date</span></span>
- <span data-ttu-id="9b04d-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="9b04d-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="9b04d-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b04d-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9b04d-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b04d-153">Request</span></span>

<span data-ttu-id="9b04d-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b04d-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9b04d-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b04d-155">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9b04d-156">C#</span><span class="sxs-lookup"><span data-stu-id="9b04d-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b04d-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b04d-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9b04d-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b04d-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9b04d-159">Java</span><span class="sxs-lookup"><span data-stu-id="9b04d-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b04d-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b04d-160">Response</span></span>

<span data-ttu-id="9b04d-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b04d-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="9b04d-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="9b04d-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
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
