---
title: 'reportRoot: getOffice365ActivationCounts'
description: Obter a contagem de Microsoft 365 ativações em desktops e dispositivos.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 21444eddb72e12f52d1ab462e649be87436ff0ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049797"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="38288-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="38288-103">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="38288-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38288-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38288-105">Obter a contagem de Microsoft 365 ativações em desktops e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="38288-105">Get the count of Microsoft 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="38288-106">**Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Microsoft Office ativações](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="38288-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="38288-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="38288-107">Permissions</span></span>

<span data-ttu-id="38288-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38288-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38288-110">Permission type</span></span>                        | <span data-ttu-id="38288-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38288-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="38288-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38288-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="38288-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38288-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="38288-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38288-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38288-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38288-115">Not supported.</span></span>                           |
| <span data-ttu-id="38288-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38288-116">Application</span></span>                            | <span data-ttu-id="38288-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38288-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="38288-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="38288-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="38288-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="38288-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="38288-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38288-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="38288-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="38288-121">Query parameters</span></span>

<span data-ttu-id="38288-122">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="38288-122">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="38288-123">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="38288-123">The default output type is text/csv.</span></span> <span data-ttu-id="38288-124">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="38288-124">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38288-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38288-125">Request headers</span></span>

| <span data-ttu-id="38288-126">Nome</span><span class="sxs-lookup"><span data-stu-id="38288-126">Name</span></span>          | <span data-ttu-id="38288-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="38288-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="38288-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="38288-128">Authorization</span></span> | <span data-ttu-id="38288-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38288-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="38288-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="38288-131">Response</span></span>

### <a name="csv"></a><span data-ttu-id="38288-132">CSV</span><span class="sxs-lookup"><span data-stu-id="38288-132">CSV</span></span>

<span data-ttu-id="38288-133">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="38288-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="38288-134">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="38288-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="38288-135">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="38288-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="38288-136">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="38288-136">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="38288-137">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="38288-137">Report Refresh Date</span></span>
- <span data-ttu-id="38288-138">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="38288-138">Product Type</span></span>
- <span data-ttu-id="38288-139">Windows</span><span class="sxs-lookup"><span data-stu-id="38288-139">Windows</span></span>
- <span data-ttu-id="38288-140">Mac</span><span class="sxs-lookup"><span data-stu-id="38288-140">Mac</span></span>
- <span data-ttu-id="38288-141">Android</span><span class="sxs-lookup"><span data-stu-id="38288-141">Android</span></span>
- <span data-ttu-id="38288-142">iOS</span><span class="sxs-lookup"><span data-stu-id="38288-142">iOS</span></span>
- <span data-ttu-id="38288-143">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="38288-143">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="38288-144">JSON</span><span class="sxs-lookup"><span data-stu-id="38288-144">JSON</span></span>

<span data-ttu-id="38288-145">Se tiver êxito, este método retornará um código de resposta e um `200 OK` **[objeto office365ActivationCounts](../resources/office365activationcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38288-145">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38288-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38288-146">Example</span></span>

### <a name="csv"></a><span data-ttu-id="38288-147">CSV</span><span class="sxs-lookup"><span data-stu-id="38288-147">CSV</span></span>

<span data-ttu-id="38288-148">A seguir, um exemplo que dá saída ao CSV.</span><span class="sxs-lookup"><span data-stu-id="38288-148">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="38288-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38288-149">Request</span></span>

<span data-ttu-id="38288-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38288-150">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="38288-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="38288-151">Response</span></span>

<span data-ttu-id="38288-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38288-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="38288-153">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="38288-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```

### <a name="json"></a><span data-ttu-id="38288-154">JSON</span><span class="sxs-lookup"><span data-stu-id="38288-154">JSON</span></span>

<span data-ttu-id="38288-155">A seguir, um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="38288-155">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="38288-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38288-156">Request</span></span>

<span data-ttu-id="38288-157">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="38288-157">The following example shows the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="38288-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="38288-158">Response</span></span>

<span data-ttu-id="38288-159">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="38288-159">The following example shows the response.</span></span>

> <span data-ttu-id="38288-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="38288-160">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Microsoft 365 Apps for enterprise", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
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


