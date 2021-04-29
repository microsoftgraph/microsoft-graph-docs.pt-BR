---
title: 'configurações: resetToDefault'
description: Redefine as configurações de caso para os valores padrão.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 331e5aa2e104e53c9de67cd97a3802e2ae7d8e79
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080704"
---
# <a name="settings-resettodefault"></a><span data-ttu-id="b589d-103">configurações: resetToDefault</span><span class="sxs-lookup"><span data-stu-id="b589d-103">settings: resetToDefault</span></span>

<span data-ttu-id="b589d-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b589d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b589d-105">Redefinir as configurações de caso para os valores padrão.</span><span class="sxs-lookup"><span data-stu-id="b589d-105">Reset the case settings to the default values.</span></span>

## <a name="permissions"></a><span data-ttu-id="b589d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b589d-106">Permissions</span></span>

<span data-ttu-id="b589d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b589d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b589d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b589d-109">Permission type</span></span>|<span data-ttu-id="b589d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b589d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b589d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b589d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b589d-112">eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b589d-112">eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="b589d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b589d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b589d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b589d-114">Not supported.</span></span>|
|<span data-ttu-id="b589d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b589d-115">Application</span></span>|<span data-ttu-id="b589d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b589d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b589d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b589d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/settings/resetToDefault
```

## <a name="request-headers"></a><span data-ttu-id="b589d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b589d-118">Request headers</span></span>

|<span data-ttu-id="b589d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b589d-119">Name</span></span>|<span data-ttu-id="b589d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b589d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b589d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b589d-121">Authorization</span></span>|<span data-ttu-id="b589d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b589d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b589d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b589d-124">Request body</span></span>

<span data-ttu-id="b589d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b589d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b589d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b589d-126">Response</span></span>

<span data-ttu-id="b589d-127">Se tiver êxito, esta ação retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="b589d-127">If successful, this action returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b589d-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b589d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b589d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b589d-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "settings_resettodefault"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/settings/resetToDefault
```

### <a name="response"></a><span data-ttu-id="b589d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b589d-130">Response</span></span>

<span data-ttu-id="b589d-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b589d-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
