---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Obtenha a contagem de usuários por tipo de atividade e serviço.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f979a9a13fdd5cd8b35d75d3549fe69931d0823c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864408"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="1bca2-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="1bca2-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="1bca2-104">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="1bca2-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="1bca2-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="1bca2-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="1bca2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1bca2-106">Permissions</span></span>

<span data-ttu-id="1bca2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bca2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1bca2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bca2-109">Permission type</span></span>                        | <span data-ttu-id="1bca2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1bca2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1bca2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bca2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1bca2-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bca2-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1bca2-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bca2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bca2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bca2-114">Not supported.</span></span>                           |
| <span data-ttu-id="1bca2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-115">Application</span></span>                            | <span data-ttu-id="1bca2-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bca2-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="1bca2-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="1bca2-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="1bca2-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="1bca2-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="1bca2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bca2-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1bca2-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="1bca2-120">Function parameters</span></span>

<span data-ttu-id="1bca2-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1bca2-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1bca2-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1bca2-122">Parameter</span></span> | <span data-ttu-id="1bca2-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bca2-123">Type</span></span>   | <span data-ttu-id="1bca2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bca2-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1bca2-125">ponto</span><span class="sxs-lookup"><span data-stu-id="1bca2-125">period</span></span>    | <span data-ttu-id="1bca2-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bca2-126">string</span></span> | <span data-ttu-id="1bca2-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1bca2-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1bca2-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="1bca2-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1bca2-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1bca2-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1bca2-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bca2-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1bca2-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bca2-131">Request headers</span></span>

| <span data-ttu-id="1bca2-132">Nome</span><span class="sxs-lookup"><span data-stu-id="1bca2-132">Name</span></span>          | <span data-ttu-id="1bca2-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bca2-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1bca2-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bca2-134">Authorization</span></span> | <span data-ttu-id="1bca2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bca2-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1bca2-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1bca2-137">If-None-Match</span></span> | <span data-ttu-id="1bca2-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="1bca2-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1bca2-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1bca2-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1bca2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bca2-140">Response</span></span>

<span data-ttu-id="1bca2-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="1bca2-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1bca2-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1bca2-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1bca2-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1bca2-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1bca2-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="1bca2-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1bca2-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="1bca2-145">Report Refresh Date</span></span>
- <span data-ttu-id="1bca2-146">Exchange ativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-146">Exchange Active</span></span>
- <span data-ttu-id="1bca2-147">Exchange inativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-147">Exchange Inactive</span></span>
- <span data-ttu-id="1bca2-148">OneDrive ativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-148">OneDrive Active</span></span>
- <span data-ttu-id="1bca2-149">OneDrive inativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-149">OneDrive Inactive</span></span>
- <span data-ttu-id="1bca2-150">SharePoint ativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-150">SharePoint Active</span></span>
- <span data-ttu-id="1bca2-151">SharePoint inativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-151">SharePoint Inactive</span></span>
- <span data-ttu-id="1bca2-152">Skype for Business ativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-152">Skype For Business Active</span></span>
- <span data-ttu-id="1bca2-153">Skype for Business inativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-153">Skype For Business Inactive</span></span>
- <span data-ttu-id="1bca2-154">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="1bca2-154">Yammer Active</span></span>
- <span data-ttu-id="1bca2-155">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="1bca2-155">Yammer Inactive</span></span>
- <span data-ttu-id="1bca2-156">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-156">Teams Active</span></span>
- <span data-ttu-id="1bca2-157">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-157">Teams Inactive</span></span>
- <span data-ttu-id="1bca2-158">Office 365 active</span><span class="sxs-lookup"><span data-stu-id="1bca2-158">Office 365 Active</span></span>
- <span data-ttu-id="1bca2-159">Office 365 inativo</span><span class="sxs-lookup"><span data-stu-id="1bca2-159">Office 365 Inactive</span></span>
- <span data-ttu-id="1bca2-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="1bca2-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1bca2-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bca2-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1bca2-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bca2-162">Request</span></span>

<span data-ttu-id="1bca2-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bca2-163">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1bca2-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bca2-164">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1bca2-165">C#</span><span class="sxs-lookup"><span data-stu-id="1bca2-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bca2-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bca2-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1bca2-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bca2-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1bca2-168">Java</span><span class="sxs-lookup"><span data-stu-id="1bca2-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365servicesusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1bca2-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bca2-169">Response</span></span>

<span data-ttu-id="1bca2-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1bca2-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="1bca2-171">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="1bca2-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Office 365 Active,Office 365 Inactive,Report Period
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
