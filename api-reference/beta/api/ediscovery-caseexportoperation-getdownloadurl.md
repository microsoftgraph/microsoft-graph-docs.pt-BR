---
title: 'caseExportOperation: getDownloadUrl'
description: 'Retorna a URL de download '
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f05c7a63dce306ff07993e6111a9323c6a14d599
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445814"
---
# <a name="caseexportoperation-getdownloadurl"></a><span data-ttu-id="54bf6-103">caseExportOperation: getDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="54bf6-103">caseExportOperation: getDownloadUrl</span></span>

<span data-ttu-id="54bf6-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="54bf6-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54bf6-105">Retorna a URL de download de uma exportação quando a exportação estiver pronta.</span><span class="sxs-lookup"><span data-stu-id="54bf6-105">Returns the download URL for an export when the export is ready.</span></span>

## <a name="permissions"></a><span data-ttu-id="54bf6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="54bf6-106">Permissions</span></span>

<span data-ttu-id="54bf6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54bf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54bf6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54bf6-109">Permission type</span></span>|<span data-ttu-id="54bf6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54bf6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54bf6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54bf6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="54bf6-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54bf6-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="54bf6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54bf6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54bf6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54bf6-114">Not supported.</span></span>|
|<span data-ttu-id="54bf6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54bf6-115">Application</span></span>|<span data-ttu-id="54bf6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54bf6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54bf6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54bf6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/operations/{operationId}/microsoft.graph.ediscovery.caseExportOperation/getDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="54bf6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54bf6-118">Request headers</span></span>
|<span data-ttu-id="54bf6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="54bf6-119">Name</span></span>|<span data-ttu-id="54bf6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="54bf6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="54bf6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="54bf6-121">Authorization</span></span>|<span data-ttu-id="54bf6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54bf6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="54bf6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54bf6-124">Request body</span></span>
<span data-ttu-id="54bf6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54bf6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54bf6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="54bf6-126">Response</span></span>

<span data-ttu-id="54bf6-127">Se tiver êxito, essa função retornará `200 OK` um código de resposta e um String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54bf6-127">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span> <span data-ttu-id="54bf6-128">O campo valor representa a URL de download de onde a exportação pode ser recuperada.</span><span class="sxs-lookup"><span data-stu-id="54bf6-128">The value field represents the download URL from where the export can be retrieved.</span></span>

## <a name="examples"></a><span data-ttu-id="54bf6-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="54bf6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54bf6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54bf6-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "caseexportoperation_getdownloadurl"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/operations/63926d4779c243458902328d83f61f53/microsoft.graph.ediscovery.caseExportOperation/getDownloadUrl
```

### <a name="response"></a><span data-ttu-id="54bf6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="54bf6-131">Response</span></span>

<span data-ttu-id="54bf6-132">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="54bf6-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.String"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Edm.String",
    "value": "https://nam01pkgg0052.blob.edproxy.nam01.ediscovery.outlook.com/packaging0041e27c6c924a48befe348d34066c25/d0b6d2a7-5fc5-44f0-9bca-6b9d34a9410b.zip?sv=2018-03-28&sr=c&sig=TRFQNUGFtuVO7zd39oNJjzcQYJus2TXY%2B50aed4pJJM%3D&se=2020-12-28T23%3A06%3A26Z&sp=racwdl"
}
```
