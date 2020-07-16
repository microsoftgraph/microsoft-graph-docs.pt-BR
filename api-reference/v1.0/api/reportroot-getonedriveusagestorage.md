---
title: 'reportRoot: getOneDriveUsageStorage'
description: Obtenha a tendência da quantidade de armazenamento que você está usando no OneDrive for Business.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: cd8be2c3840b971dae82db839c05983b25ba0069
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895941"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="a4f00-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="a4f00-103">reportRoot: getOneDriveUsageStorage</span></span>

<span data-ttu-id="a4f00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4f00-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4f00-105">Obtenha a tendência da quantidade de armazenamento que você está usando no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a4f00-105">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="a4f00-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição de relatórios e nomes, consulte [Microsoft 365 Reports-uso do onedrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="a4f00-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4f00-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4f00-107">Permissions</span></span>

<span data-ttu-id="a4f00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4f00-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4f00-110">Permission type</span></span>                        | <span data-ttu-id="a4f00-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4f00-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a4f00-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4f00-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4f00-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4f00-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a4f00-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4f00-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4f00-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4f00-115">Not supported.</span></span>                           |
| <span data-ttu-id="a4f00-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4f00-116">Application</span></span>                            | <span data-ttu-id="a4f00-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4f00-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a4f00-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="a4f00-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a4f00-119">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a4f00-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a4f00-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4f00-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a4f00-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a4f00-121">Function parameters</span></span>

<span data-ttu-id="a4f00-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a4f00-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a4f00-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a4f00-123">Parameter</span></span> | <span data-ttu-id="a4f00-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4f00-124">Type</span></span>   | <span data-ttu-id="a4f00-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4f00-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a4f00-126">ponto</span><span class="sxs-lookup"><span data-stu-id="a4f00-126">period</span></span>    | <span data-ttu-id="a4f00-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4f00-127">string</span></span> | <span data-ttu-id="a4f00-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a4f00-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a4f00-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a4f00-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a4f00-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a4f00-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a4f00-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4f00-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a4f00-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4f00-132">Request headers</span></span>

| <span data-ttu-id="a4f00-133">Nome</span><span class="sxs-lookup"><span data-stu-id="a4f00-133">Name</span></span>          | <span data-ttu-id="a4f00-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4f00-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a4f00-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4f00-135">Authorization</span></span> | <span data-ttu-id="a4f00-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4f00-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a4f00-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a4f00-138">If-None-Match</span></span> | <span data-ttu-id="a4f00-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="a4f00-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a4f00-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a4f00-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a4f00-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4f00-141">Response</span></span>

<span data-ttu-id="a4f00-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a4f00-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a4f00-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a4f00-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a4f00-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a4f00-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a4f00-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a4f00-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a4f00-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a4f00-146">Report Refresh Date</span></span>
- <span data-ttu-id="a4f00-147">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="a4f00-147">Site Type</span></span>
- <span data-ttu-id="a4f00-148">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="a4f00-148">Storage Used (Byte)</span></span>
- <span data-ttu-id="a4f00-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="a4f00-149">Report Date</span></span>
- <span data-ttu-id="a4f00-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a4f00-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a4f00-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4f00-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a4f00-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4f00-152">Request</span></span>

<span data-ttu-id="a4f00-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4f00-153">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getonedriveusagestorage"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageStorage(period='D7')
```


#### <a name="response"></a><span data-ttu-id="a4f00-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4f00-154">Response</span></span>

<span data-ttu-id="a4f00-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a4f00-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="a4f00-156">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a4f00-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
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
