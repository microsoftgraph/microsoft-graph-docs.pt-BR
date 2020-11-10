---
title: Atualizar connectorGroups
description: Atualize as propriedades do objeto de conexão.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d376327004d77277dd418556cc8caffe2da49e8e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957267"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="bc5c6-103">Atualizar connectorGroups</span><span class="sxs-lookup"><span data-stu-id="bc5c6-103">Update connectorGroups</span></span>

<span data-ttu-id="bc5c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc5c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc5c6-105">Atualizar as propriedades de um objeto de [conexão](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="bc5c6-105">Update the properties of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc5c6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc5c6-106">Permissions</span></span>
<span data-ttu-id="bc5c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc5c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc5c6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc5c6-109">Permission type</span></span>      | <span data-ttu-id="bc5c6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc5c6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc5c6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc5c6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc5c6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc5c6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bc5c6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc5c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc5c6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-114">Not supported.</span></span>    |
|<span data-ttu-id="bc5c6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc5c6-115">Application</span></span> | <span data-ttu-id="bc5c6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bc5c6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc5c6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="bc5c6-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="bc5c6-118">Optional request headers</span></span>
| <span data-ttu-id="bc5c6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bc5c6-119">Name</span></span>       | <span data-ttu-id="bc5c6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc5c6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bc5c6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc5c6-121">Authorization</span></span>  | <span data-ttu-id="bc5c6-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-122">Bearer.</span></span> <span data-ttu-id="bc5c6-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="bc5c6-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc5c6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc5c6-124">Request body</span></span>
<span data-ttu-id="bc5c6-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bc5c6-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc5c6-128">Property</span></span>     | <span data-ttu-id="bc5c6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc5c6-129">Type</span></span>   |<span data-ttu-id="bc5c6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc5c6-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc5c6-131">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="bc5c6-131">connectorGroupType</span></span>|<span data-ttu-id="bc5c6-132">string</span><span class="sxs-lookup"><span data-stu-id="bc5c6-132">string</span></span>| <span data-ttu-id="bc5c6-133">Indica o tipo de agente híbrido.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-133">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="bc5c6-134">Isso é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-134">This pre-set by the system.</span></span> |
|<span data-ttu-id="bc5c6-135">id</span><span class="sxs-lookup"><span data-stu-id="bc5c6-135">id</span></span>|<span data-ttu-id="bc5c6-136">string</span><span class="sxs-lookup"><span data-stu-id="bc5c6-136">string</span></span>| <span data-ttu-id="bc5c6-137">Identificador exclusivo desse conector.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-137">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="bc5c6-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-138">Read-only.</span></span> |
|<span data-ttu-id="bc5c6-139">isDefault</span><span class="sxs-lookup"><span data-stu-id="bc5c6-139">isDefault</span></span>|<span data-ttu-id="bc5c6-140">booliano</span><span class="sxs-lookup"><span data-stu-id="bc5c6-140">boolean</span></span>| <span data-ttu-id="bc5c6-141">Indica se o conector de conexão é o padrão.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-141">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="bc5c6-142">Somente um grupo de conectores único pode ser o grupo de conectores padrão e é predefinido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-142">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> |
|<span data-ttu-id="bc5c6-143">nome</span><span class="sxs-lookup"><span data-stu-id="bc5c6-143">name</span></span>|<span data-ttu-id="bc5c6-144">string</span><span class="sxs-lookup"><span data-stu-id="bc5c6-144">string</span></span>| <span data-ttu-id="bc5c6-145">O nome associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-145">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="bc5c6-146">região</span><span class="sxs-lookup"><span data-stu-id="bc5c6-146">region</span></span>|<span data-ttu-id="bc5c6-147">string</span><span class="sxs-lookup"><span data-stu-id="bc5c6-147">string</span></span>| <span data-ttu-id="bc5c6-148">A região à qual o conector é atribuído e otimizará o tráfego para o.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-148">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="bc5c6-149">Essa região só poderá ser definida se **nenhum** conector ou aplicativo for atribuído ao grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-149">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="bc5c6-150">As regiões disponíveis incluem: América do Norte, Europa, Austrália, Ásia e Índia.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-150">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="bc5c6-151">Os valores possíveis são: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-151">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="bc5c6-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc5c6-152">Response</span></span>

<span data-ttu-id="bc5c6-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [teleconnector](../resources/connectorgroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-153">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc5c6-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc5c6-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc5c6-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc5c6-155">Request</span></span>
<span data-ttu-id="bc5c6-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc5c6-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc5c6-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "region": "region-value"
}
```
# <a name="c"></a>[<span data-ttu-id="bc5c6-158">C#</span><span class="sxs-lookup"><span data-stu-id="bc5c6-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc5c6-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc5c6-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc5c6-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc5c6-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc5c6-161">Java</span><span class="sxs-lookup"><span data-stu-id="bc5c6-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bc5c6-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc5c6-162">Response</span></span>
<span data-ttu-id="bc5c6-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-163">The following is an example of the response.</span></span> <span data-ttu-id="bc5c6-164">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bc5c6-165">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc5c6-165">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true,
  "region": "region-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


