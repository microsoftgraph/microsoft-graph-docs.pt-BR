---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office em desktops ou dispositivos ou computadores compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 22caf9e7897f2f3646921707d6d333c5e5da38fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454399"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="d862e-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="d862e-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="d862e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d862e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d862e-105">Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office em desktops ou dispositivos ou computadores compartilhados.</span><span class="sxs-lookup"><span data-stu-id="d862e-105">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="d862e-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="d862e-106">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="d862e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d862e-107">Permissions</span></span>

<span data-ttu-id="d862e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d862e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d862e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d862e-110">Permission type</span></span>                        | <span data-ttu-id="d862e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d862e-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d862e-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d862e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d862e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d862e-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d862e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d862e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d862e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d862e-115">Not supported.</span></span>                           |
| <span data-ttu-id="d862e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d862e-116">Application</span></span>                            | <span data-ttu-id="d862e-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d862e-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="d862e-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d862e-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d862e-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="d862e-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d862e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d862e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="query-parameters"></a><span data-ttu-id="d862e-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="d862e-121">Query parameters</span></span>

<span data-ttu-id="d862e-122">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d862e-122">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d862e-123">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="d862e-123">The default output type is text/csv.</span></span> <span data-ttu-id="d862e-124">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d862e-124">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d862e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d862e-125">Request headers</span></span>

| <span data-ttu-id="d862e-126">Nome</span><span class="sxs-lookup"><span data-stu-id="d862e-126">Name</span></span>          | <span data-ttu-id="d862e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d862e-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d862e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d862e-128">Authorization</span></span> | <span data-ttu-id="d862e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d862e-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d862e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d862e-131">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d862e-132">CSV</span><span class="sxs-lookup"><span data-stu-id="d862e-132">CSV</span></span>

<span data-ttu-id="d862e-133">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d862e-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d862e-134">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d862e-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d862e-135">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d862e-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d862e-136">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d862e-136">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d862e-137">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d862e-137">Report Refresh Date</span></span>
- <span data-ttu-id="d862e-138">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="d862e-138">Product Type</span></span>
- <span data-ttu-id="d862e-139">Atribuído</span><span class="sxs-lookup"><span data-stu-id="d862e-139">Assigned</span></span>
- <span data-ttu-id="d862e-140">Ativado</span><span class="sxs-lookup"><span data-stu-id="d862e-140">Activated</span></span>
- <span data-ttu-id="d862e-141">Ativação de computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="d862e-141">Shared Computer Activation</span></span>

### <a name="json"></a><span data-ttu-id="d862e-142">JSON</span><span class="sxs-lookup"><span data-stu-id="d862e-142">JSON</span></span>

<span data-ttu-id="d862e-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d862e-143">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d862e-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d862e-144">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d862e-145">CSV</span><span class="sxs-lookup"><span data-stu-id="d862e-145">CSV</span></span>

<span data-ttu-id="d862e-146">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="d862e-146">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d862e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d862e-147">Request</span></span>

<span data-ttu-id="d862e-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d862e-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d862e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="d862e-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="d862e-150">C#</span><span class="sxs-lookup"><span data-stu-id="d862e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d862e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d862e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d862e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d862e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d862e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d862e-153">Response</span></span>

<span data-ttu-id="d862e-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d862e-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d862e-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d862e-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```

### <a name="json"></a><span data-ttu-id="d862e-156">JSON</span><span class="sxs-lookup"><span data-stu-id="d862e-156">JSON</span></span>

<span data-ttu-id="d862e-157">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="d862e-157">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d862e-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d862e-158">Request</span></span>

<span data-ttu-id="d862e-159">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d862e-159">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d862e-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="d862e-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="d862e-161">C#</span><span class="sxs-lookup"><span data-stu-id="d862e-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d862e-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d862e-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d862e-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d862e-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d862e-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="d862e-164">Response</span></span>

<span data-ttu-id="d862e-165">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="d862e-165">The following example shows the response.</span></span>

> <span data-ttu-id="d862e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d862e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "assigned": 2679, 
      "activated": 1710,
      "sharedComputerActivation": 1024
    }
  ]
}
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
