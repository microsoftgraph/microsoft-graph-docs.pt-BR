---
title: 'reportRoot: getOffice365ActivationCounts'
description: Obtenha a contagem de ativações do Office 365 em desktops e dispositivos.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 635b3bf4ff66aee2ea792fa9bfaedd936447ea16
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571412"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="c5580-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="c5580-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5580-104">Obtenha a contagem de ativações do Office 365 em desktops e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="c5580-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="c5580-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="c5580-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5580-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5580-106">Permissions</span></span>

<span data-ttu-id="c5580-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5580-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5580-109">Permission type</span></span>                        | <span data-ttu-id="c5580-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5580-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c5580-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5580-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5580-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5580-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c5580-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5580-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5580-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5580-114">Not supported.</span></span>                           |
| <span data-ttu-id="c5580-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5580-115">Application</span></span>                            | <span data-ttu-id="c5580-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5580-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c5580-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5580-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="c5580-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="c5580-118">Query parameters</span></span>

<span data-ttu-id="c5580-119">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5580-119">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c5580-120">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="c5580-120">The default output type is text/csv.</span></span> <span data-ttu-id="c5580-121">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="c5580-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5580-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5580-122">Request headers</span></span>

| <span data-ttu-id="c5580-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c5580-123">Name</span></span>          | <span data-ttu-id="c5580-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5580-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c5580-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5580-125">Authorization</span></span> | <span data-ttu-id="c5580-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5580-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c5580-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5580-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c5580-129">CSV</span><span class="sxs-lookup"><span data-stu-id="c5580-129">CSV</span></span>

<span data-ttu-id="c5580-130">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="c5580-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c5580-131">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c5580-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c5580-132">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c5580-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c5580-133">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="c5580-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c5580-134">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="c5580-134">Report Refresh Date</span></span>
- <span data-ttu-id="c5580-135">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="c5580-135">Product Type</span></span>
- <span data-ttu-id="c5580-136">Windows</span><span class="sxs-lookup"><span data-stu-id="c5580-136">Windows</span></span>
- <span data-ttu-id="c5580-137">Mac</span><span class="sxs-lookup"><span data-stu-id="c5580-137">Mac</span></span>
- <span data-ttu-id="c5580-138">Android</span><span class="sxs-lookup"><span data-stu-id="c5580-138">Android</span></span>
- <span data-ttu-id="c5580-139">iOS</span><span class="sxs-lookup"><span data-stu-id="c5580-139">iOS</span></span>
- <span data-ttu-id="c5580-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="c5580-140">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="c5580-141">JSON</span><span class="sxs-lookup"><span data-stu-id="c5580-141">JSON</span></span>

<span data-ttu-id="c5580-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365ActivationCounts](../resources/office365activationcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5580-142">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5580-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5580-143">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c5580-144">CSV</span><span class="sxs-lookup"><span data-stu-id="c5580-144">CSV</span></span>

<span data-ttu-id="c5580-145">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="c5580-145">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c5580-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5580-146">Request</span></span>

<span data-ttu-id="c5580-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5580-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c5580-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5580-148">Response</span></span>

<span data-ttu-id="c5580-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5580-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c5580-150">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="c5580-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="c5580-151">JSON</span><span class="sxs-lookup"><span data-stu-id="c5580-151">JSON</span></span>

<span data-ttu-id="c5580-152">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="c5580-152">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c5580-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5580-153">Request</span></span>

<span data-ttu-id="c5580-154">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5580-154">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c5580-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5580-155">Response</span></span>

<span data-ttu-id="c5580-156">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5580-156">The following example shows the response.</span></span>

> <span data-ttu-id="c5580-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5580-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "productType": "Office 365 ProPlus", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activationcounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
