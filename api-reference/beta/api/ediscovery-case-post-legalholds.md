---
title: Criar legalHold
description: Crie um novo objeto legalHold.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f004302998c5c65164c3d8ace3778d8bd75a6984
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445828"
---
# <a name="create-legalhold"></a><span data-ttu-id="d9437-103">Criar legalHold</span><span class="sxs-lookup"><span data-stu-id="d9437-103">Create legalHold</span></span>

<span data-ttu-id="d9437-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d9437-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9437-105">Crie um novo [objeto legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="d9437-105">Create a new [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9437-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9437-106">Permissions</span></span>

<span data-ttu-id="d9437-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9437-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9437-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9437-109">Permission type</span></span>|<span data-ttu-id="d9437-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9437-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9437-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9437-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9437-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9437-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d9437-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9437-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9437-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9437-114">Not supported.</span></span>|
|<span data-ttu-id="d9437-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9437-115">Application</span></span>|<span data-ttu-id="d9437-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9437-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9437-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9437-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds
```

## <a name="request-headers"></a><span data-ttu-id="d9437-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9437-118">Request headers</span></span>

|<span data-ttu-id="d9437-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d9437-119">Name</span></span>|<span data-ttu-id="d9437-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9437-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d9437-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9437-121">Authorization</span></span>|<span data-ttu-id="d9437-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9437-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d9437-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9437-124">Content-Type</span></span>|<span data-ttu-id="d9437-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9437-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9437-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9437-127">Request body</span></span>

<span data-ttu-id="d9437-128">No corpo da solicitação, fornece uma representação JSON do [objeto legalHold.](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="d9437-128">In the request body, supply a JSON representation of the [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

<span data-ttu-id="d9437-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [legalHold](../resources/ediscovery-legalhold.md).</span><span class="sxs-lookup"><span data-stu-id="d9437-129">The following table shows the properties that are required when you create the [legalHold](../resources/ediscovery-legalhold.md).</span></span>

|<span data-ttu-id="d9437-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9437-130">Property</span></span>|<span data-ttu-id="d9437-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9437-131">Type</span></span>|<span data-ttu-id="d9437-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9437-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9437-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d9437-133">displayName</span></span>|<span data-ttu-id="d9437-134">String</span><span class="sxs-lookup"><span data-stu-id="d9437-134">String</span></span>| <span data-ttu-id="d9437-135">O nome de exibição da ressução legal.</span><span class="sxs-lookup"><span data-stu-id="d9437-135">The display name of the legal hold.</span></span> |

## <a name="response"></a><span data-ttu-id="d9437-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9437-136">Response</span></span>

<span data-ttu-id="d9437-137">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9437-137">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9437-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d9437-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9437-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9437-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_legalhold_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds
Content-Type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String"
}
```

### <a name="response"></a><span data-ttu-id="d9437-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9437-140">Response</span></span>

<span data-ttu-id="d9437-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d9437-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "id": "700cd868-d868-700c-68d8-0c7068d80c70",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
