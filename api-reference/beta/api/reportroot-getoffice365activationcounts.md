---
title: 'reportRoot: getOffice365ActivationCounts'
description: Obtenha a contagem de ativações do Office 365 em desktops e dispositivos.
ms.openlocfilehash: c75b957f02eb5d5fa77f5e3dfa696f3086f9d817
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034738"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="0d9ba-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="0d9ba-103">reportRoot: getOffice365ActivationCounts</span></span>

> <span data-ttu-id="0d9ba-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d9ba-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d9ba-106">Obtenha a contagem de ativações do Office 365 em desktops e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-106">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="0d9ba-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="0d9ba-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d9ba-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d9ba-108">Permissions</span></span>

<span data-ttu-id="0d9ba-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d9ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d9ba-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d9ba-111">Permission type</span></span>                        | <span data-ttu-id="0d9ba-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d9ba-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0d9ba-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d9ba-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d9ba-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d9ba-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0d9ba-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d9ba-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d9ba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-116">Not supported.</span></span>                           |
| <span data-ttu-id="0d9ba-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d9ba-117">Application</span></span>                            | <span data-ttu-id="0d9ba-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d9ba-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0d9ba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d9ba-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="0d9ba-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="0d9ba-120">Query parameters</span></span>

<span data-ttu-id="0d9ba-121">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0d9ba-122">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-122">The default output type is text/csv.</span></span> <span data-ttu-id="0d9ba-123">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d9ba-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d9ba-124">Request headers</span></span>

| <span data-ttu-id="0d9ba-125">Nome</span><span class="sxs-lookup"><span data-stu-id="0d9ba-125">Name</span></span>          | <span data-ttu-id="0d9ba-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d9ba-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0d9ba-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d9ba-127">Authorization</span></span> | <span data-ttu-id="0d9ba-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0d9ba-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d9ba-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0d9ba-131">CSV</span><span class="sxs-lookup"><span data-stu-id="0d9ba-131">CSV</span></span>

<span data-ttu-id="0d9ba-132">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0d9ba-133">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0d9ba-134">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0d9ba-135">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0d9ba-136">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="0d9ba-136">Report Refresh Date</span></span>
- <span data-ttu-id="0d9ba-137">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="0d9ba-137">Product Type</span></span>
- <span data-ttu-id="0d9ba-138">Windows</span><span class="sxs-lookup"><span data-stu-id="0d9ba-138">Windows</span></span>
- <span data-ttu-id="0d9ba-139">Mac</span><span class="sxs-lookup"><span data-stu-id="0d9ba-139">Mac</span></span>
- <span data-ttu-id="0d9ba-140">Android</span><span class="sxs-lookup"><span data-stu-id="0d9ba-140">Android</span></span>
- <span data-ttu-id="0d9ba-141">iOS</span><span class="sxs-lookup"><span data-stu-id="0d9ba-141">iOS</span></span>
- <span data-ttu-id="0d9ba-142">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="0d9ba-142">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="0d9ba-143">JSON</span><span class="sxs-lookup"><span data-stu-id="0d9ba-143">JSON</span></span>

<span data-ttu-id="0d9ba-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365ActivationCounts](../resources/office365activationcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-144">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d9ba-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d9ba-145">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0d9ba-146">CSV</span><span class="sxs-lookup"><span data-stu-id="0d9ba-146">CSV</span></span>

<span data-ttu-id="0d9ba-147">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-147">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0d9ba-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d9ba-148">Request</span></span>

<span data-ttu-id="0d9ba-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0d9ba-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d9ba-150">Response</span></span>

<span data-ttu-id="0d9ba-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-151">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0d9ba-152">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="0d9ba-153">JSON</span><span class="sxs-lookup"><span data-stu-id="0d9ba-153">JSON</span></span>

<span data-ttu-id="0d9ba-154">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-154">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0d9ba-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d9ba-155">Request</span></span>

<span data-ttu-id="0d9ba-156">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-156">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0d9ba-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d9ba-157">Response</span></span>

<span data-ttu-id="0d9ba-158">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-158">The following example shows the response.</span></span>

> <span data-ttu-id="0d9ba-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d9ba-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
