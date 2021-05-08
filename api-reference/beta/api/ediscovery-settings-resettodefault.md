---
title: 'configurações: resetToDefault'
description: Redefine as configurações de caso para os valores padrão.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3bc0cbcad51243e7f264ce69e92370cba864df54
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239658"
---
# <a name="settings-resettodefault"></a><span data-ttu-id="9cd76-103">configurações: resetToDefault</span><span class="sxs-lookup"><span data-stu-id="9cd76-103">settings: resetToDefault</span></span>

<span data-ttu-id="9cd76-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="9cd76-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cd76-105">Redefinir as configurações de caso para os valores padrão.</span><span class="sxs-lookup"><span data-stu-id="9cd76-105">Reset the case settings to the default values.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cd76-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cd76-106">Permissions</span></span>

<span data-ttu-id="9cd76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cd76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cd76-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cd76-109">Permission type</span></span>|<span data-ttu-id="9cd76-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cd76-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cd76-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cd76-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9cd76-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cd76-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="9cd76-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cd76-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cd76-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cd76-114">Not supported.</span></span>|
|<span data-ttu-id="9cd76-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cd76-115">Application</span></span>|<span data-ttu-id="9cd76-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cd76-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cd76-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cd76-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/settings/resetToDefault
```

## <a name="request-headers"></a><span data-ttu-id="9cd76-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cd76-118">Request headers</span></span>

|<span data-ttu-id="9cd76-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9cd76-119">Name</span></span>|<span data-ttu-id="9cd76-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cd76-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9cd76-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cd76-121">Authorization</span></span>|<span data-ttu-id="9cd76-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cd76-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cd76-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cd76-124">Request body</span></span>

<span data-ttu-id="9cd76-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9cd76-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cd76-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cd76-126">Response</span></span>

<span data-ttu-id="9cd76-127">Se tiver êxito, esta ação retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="9cd76-127">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9cd76-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9cd76-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9cd76-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cd76-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9cd76-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cd76-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "settings_resettodefault"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/settings/resetToDefault
```
# <a name="c"></a>[<span data-ttu-id="9cd76-131">C#</span><span class="sxs-lookup"><span data-stu-id="9cd76-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/settings-resettodefault-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cd76-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cd76-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/settings-resettodefault-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cd76-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cd76-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/settings-resettodefault-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cd76-134">Java</span><span class="sxs-lookup"><span data-stu-id="9cd76-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/settings-resettodefault-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9cd76-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cd76-135">Response</span></span>

<span data-ttu-id="9cd76-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9cd76-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.settings"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/settings/$entity",
    "id": "5b840b94-f821-4c4a-8cad-3a90062bf51a",
    "redundancyDetection": {
        "isEnabled": true,
        "similarityThreshold": 65,
        "minWords": 10,
        "maxWords": 500000
    },
    "topicModeling": {
        "isEnabled": true,
        "ignoreNumbers": true,
        "topicCount": 100,
        "dynamicallyAdjustTopicCount": true
    },
    "ocr": {
        "isEnabled": false,
        "maxImageSize": 24576,
        "timeout": "PT1M"
    }
}
```
