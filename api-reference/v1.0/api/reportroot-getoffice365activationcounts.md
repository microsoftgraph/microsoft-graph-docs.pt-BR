---
title: 'reportRoot: getOffice365ActivationCounts'
description: Obtenha a contagem de ativações do Office 365 em desktops e dispositivos.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c7e7211218a3ed5f4a9e266a6358f47318c88e05
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864457"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="333c4-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="333c4-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="333c4-104">Obtenha a contagem de ativações do Office 365 em desktops e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="333c4-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="333c4-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="333c4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="333c4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="333c4-106">Permissions</span></span>

<span data-ttu-id="333c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="333c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="333c4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="333c4-109">Permission type</span></span>                        | <span data-ttu-id="333c4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="333c4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="333c4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="333c4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="333c4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="333c4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="333c4-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="333c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="333c4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="333c4-114">Not supported.</span></span>                           |
| <span data-ttu-id="333c4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="333c4-115">Application</span></span>                            | <span data-ttu-id="333c4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="333c4-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="333c4-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="333c4-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="333c4-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="333c4-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="333c4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="333c4-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="333c4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="333c4-120">Request headers</span></span>

| <span data-ttu-id="333c4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="333c4-121">Name</span></span>          | <span data-ttu-id="333c4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="333c4-122">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="333c4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="333c4-123">Authorization</span></span> | <span data-ttu-id="333c4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="333c4-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="333c4-126">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="333c4-126">If-None-Match</span></span> | <span data-ttu-id="333c4-127">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="333c4-127">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="333c4-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="333c4-128">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="333c4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="333c4-129">Response</span></span>

<span data-ttu-id="333c4-130">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="333c4-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="333c4-131">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="333c4-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="333c4-132">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="333c4-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="333c4-133">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="333c4-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="333c4-134">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="333c4-134">Report Refresh Date</span></span>
- <span data-ttu-id="333c4-135">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="333c4-135">Product Type</span></span>
- <span data-ttu-id="333c4-136">Windows</span><span class="sxs-lookup"><span data-stu-id="333c4-136">Windows</span></span>
- <span data-ttu-id="333c4-137">Mac</span><span class="sxs-lookup"><span data-stu-id="333c4-137">Mac</span></span>
- <span data-ttu-id="333c4-138">Android</span><span class="sxs-lookup"><span data-stu-id="333c4-138">Android</span></span>
- <span data-ttu-id="333c4-139">iOS</span><span class="sxs-lookup"><span data-stu-id="333c4-139">iOS</span></span>
- <span data-ttu-id="333c4-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="333c4-140">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="333c4-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="333c4-141">Example</span></span>

#### <a name="request"></a><span data-ttu-id="333c4-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="333c4-142">Request</span></span>

<span data-ttu-id="333c4-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="333c4-143">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="333c4-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="333c4-144">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="333c4-145">C#</span><span class="sxs-lookup"><span data-stu-id="333c4-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="333c4-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="333c4-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="333c4-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="333c4-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="333c4-148">Java</span><span class="sxs-lookup"><span data-stu-id="333c4-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationcounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="333c4-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="333c4-149">Response</span></span>

<span data-ttu-id="333c4-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="333c4-150">The following is an example of the response.</span></span>

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

<span data-ttu-id="333c4-151">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="333c4-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
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
