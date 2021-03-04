---
title: Criar marca
description: Crie um novo objeto tag.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: ee08824511ffd3f32b78d5c04726686eee4d4dd4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445824"
---
# <a name="create-tag"></a><span data-ttu-id="7a59e-103">Criar marca</span><span class="sxs-lookup"><span data-stu-id="7a59e-103">Create tag</span></span>

<span data-ttu-id="7a59e-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="7a59e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a59e-105">Crie uma nova marca para o caso especificado.</span><span class="sxs-lookup"><span data-stu-id="7a59e-105">Create a new tag for the specified case.</span></span>  <span data-ttu-id="7a59e-106">As marcas são usadas em conjuntos de revisão durante a revisão do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7a59e-106">The tags are used in review sets while reviewing content.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a59e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a59e-107">Permissions</span></span>

<span data-ttu-id="7a59e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a59e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a59e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a59e-110">Permission type</span></span>|<span data-ttu-id="7a59e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a59e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a59e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a59e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a59e-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a59e-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="7a59e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a59e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a59e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a59e-115">Not supported.</span></span>|
|<span data-ttu-id="7a59e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a59e-116">Application</span></span>|<span data-ttu-id="7a59e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a59e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a59e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a59e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/tags
```

## <a name="request-headers"></a><span data-ttu-id="7a59e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a59e-119">Request headers</span></span>

|<span data-ttu-id="7a59e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7a59e-120">Name</span></span>|<span data-ttu-id="7a59e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a59e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7a59e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a59e-122">Authorization</span></span>|<span data-ttu-id="7a59e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a59e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7a59e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a59e-125">Content-Type</span></span>|<span data-ttu-id="7a59e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a59e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a59e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a59e-128">Request body</span></span>

<span data-ttu-id="7a59e-129">No corpo da solicitação, fornece uma representação JSON do [objeto tag.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="7a59e-129">In the request body, supply a JSON representation of the [tag](../resources/ediscovery-tag.md) object.</span></span>

<span data-ttu-id="7a59e-130">A tabela a seguir mostra as propriedades necessárias ao criar a [marca](../resources/ediscovery-tag.md).</span><span class="sxs-lookup"><span data-stu-id="7a59e-130">The following table shows the properties that are required when you create the [tag](../resources/ediscovery-tag.md).</span></span>

|<span data-ttu-id="7a59e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a59e-131">Property</span></span>|<span data-ttu-id="7a59e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a59e-132">Type</span></span>|<span data-ttu-id="7a59e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a59e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a59e-134">childSelectability</span><span class="sxs-lookup"><span data-stu-id="7a59e-134">childSelectability</span></span>|[<span data-ttu-id="7a59e-135">microsoft.graph.ediscovery.childSelectability</span><span class="sxs-lookup"><span data-stu-id="7a59e-135">microsoft.graph.ediscovery.childSelectability</span></span>](../resources/ediscovery-tag.md#childselectability-values)|<span data-ttu-id="7a59e-136">Indica se uma única ou várias marcas filho podem ser associadas a um documento.</span><span class="sxs-lookup"><span data-stu-id="7a59e-136">Indicates whether a single or multiple child tags can be associated with a document.</span></span> <span data-ttu-id="7a59e-137">Os valores possíveis são: `One` e `Many`.</span><span class="sxs-lookup"><span data-stu-id="7a59e-137">Possible values are: `One`, `Many`.</span></span>  <span data-ttu-id="7a59e-138">Esse valor controla se o UX apresenta as marcas como caixas de seleção ou um grupo de botões de rádio.</span><span class="sxs-lookup"><span data-stu-id="7a59e-138">This value controls whether the UX presents the tags as checkboxes or a radio button group.</span></span> <span data-ttu-id="7a59e-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a59e-139">Required.</span></span>|
|<span data-ttu-id="7a59e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7a59e-140">displayName</span></span>|<span data-ttu-id="7a59e-141">String</span><span class="sxs-lookup"><span data-stu-id="7a59e-141">String</span></span>|<span data-ttu-id="7a59e-142">Nome de exibição da marca.</span><span class="sxs-lookup"><span data-stu-id="7a59e-142">Display name of the tag.</span></span> <span data-ttu-id="7a59e-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a59e-143">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="7a59e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a59e-144">Response</span></span>

<span data-ttu-id="7a59e-145">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a59e-145">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a59e-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a59e-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a59e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a59e-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_tag_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags
Content-Type: application/json
Content-length: 235

{
  "displayName":"Privileged",
  "description":"The document is privileged",
  "parent@odata.bind":"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"
}
```

### <a name="response"></a><span data-ttu-id="7a59e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a59e-148">Response</span></span>

<span data-ttu-id="7a59e-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7a59e-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.tag"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/$entity",
    "displayName": "Privileged",
    "description": "The document is privileged",
    "lastModifiedDateTime": "2021-01-12T01:01:09.0419153Z",
    "childSelectability": "One",
    "id": "0825ef81ade74095a3b3154a3c434c3e",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```
