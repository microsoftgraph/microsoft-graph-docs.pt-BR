---
title: Atualizar connectorGroups
description: Atualize as propriedades do objeto connectorgroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: f4f74612ad071baae510d86c1e597bca0094c59f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047137"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="cae09-103">Atualizar connectorGroups</span><span class="sxs-lookup"><span data-stu-id="cae09-103">Update connectorGroups</span></span>

<span data-ttu-id="cae09-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cae09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cae09-105">Atualize as propriedades de um [objeto connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="cae09-105">Update the properties of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cae09-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cae09-106">Permissions</span></span>
<span data-ttu-id="cae09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cae09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae09-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cae09-109">Permission type</span></span>      | <span data-ttu-id="cae09-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cae09-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cae09-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cae09-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cae09-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cae09-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cae09-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cae09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae09-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cae09-114">Not supported.</span></span>    |
|<span data-ttu-id="cae09-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cae09-115">Application</span></span> | <span data-ttu-id="cae09-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cae09-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cae09-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cae09-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="cae09-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="cae09-118">Optional request headers</span></span>
| <span data-ttu-id="cae09-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cae09-119">Name</span></span>       | <span data-ttu-id="cae09-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cae09-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cae09-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cae09-121">Authorization</span></span>  | <span data-ttu-id="cae09-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="cae09-122">Bearer.</span></span> <span data-ttu-id="cae09-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="cae09-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="cae09-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cae09-124">Request body</span></span>
<span data-ttu-id="cae09-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="cae09-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cae09-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cae09-128">Property</span></span>     | <span data-ttu-id="cae09-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="cae09-129">Type</span></span>   |<span data-ttu-id="cae09-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="cae09-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cae09-131">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="cae09-131">connectorGroupType</span></span>|<span data-ttu-id="cae09-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cae09-132">string</span></span>| <span data-ttu-id="cae09-133">Indica o tipo de agente híbrido.</span><span class="sxs-lookup"><span data-stu-id="cae09-133">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="cae09-134">Este pré-definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="cae09-134">This pre-set by the system.</span></span> |
|<span data-ttu-id="cae09-135">id</span><span class="sxs-lookup"><span data-stu-id="cae09-135">id</span></span>|<span data-ttu-id="cae09-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cae09-136">string</span></span>| <span data-ttu-id="cae09-137">Identificador exclusivo para este connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="cae09-137">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="cae09-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cae09-138">Read-only.</span></span> |
|<span data-ttu-id="cae09-139">isDefault</span><span class="sxs-lookup"><span data-stu-id="cae09-139">isDefault</span></span>|<span data-ttu-id="cae09-140">booliano</span><span class="sxs-lookup"><span data-stu-id="cae09-140">boolean</span></span>| <span data-ttu-id="cae09-141">Indica se o connectorGroup é o connectorGroup padrão.</span><span class="sxs-lookup"><span data-stu-id="cae09-141">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="cae09-142">Somente um único grupo de conectores pode ser o connectorGroup padrão e isso é pré-definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="cae09-142">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> |
|<span data-ttu-id="cae09-143">nome</span><span class="sxs-lookup"><span data-stu-id="cae09-143">name</span></span>|<span data-ttu-id="cae09-144">string</span><span class="sxs-lookup"><span data-stu-id="cae09-144">string</span></span>| <span data-ttu-id="cae09-145">O nome associado ao connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="cae09-145">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="cae09-146">region</span><span class="sxs-lookup"><span data-stu-id="cae09-146">region</span></span>|<span data-ttu-id="cae09-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cae09-147">string</span></span>| <span data-ttu-id="cae09-148">A região à que o connectorGroup é atribuído e otimizará o tráfego.</span><span class="sxs-lookup"><span data-stu-id="cae09-148">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="cae09-149">Essa região só poderá ser definida se **nenhum** conector ou aplicativo for atribuído ao connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="cae09-149">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="cae09-150">As regiões disponíveis incluem: América do Norte, Europa, Austrália, Ásia e Índia.</span><span class="sxs-lookup"><span data-stu-id="cae09-150">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="cae09-151">Os valores possíveis são: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="cae09-151">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="cae09-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="cae09-152">Response</span></span>

<span data-ttu-id="cae09-153">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [connectorGroup](../resources/connectorgroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cae09-153">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cae09-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cae09-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cae09-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cae09-155">Request</span></span>
<span data-ttu-id="cae09-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cae09-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cae09-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae09-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup_2"
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
# <a name="c"></a>[<span data-ttu-id="cae09-158">C#</span><span class="sxs-lookup"><span data-stu-id="cae09-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectorgroup-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cae09-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cae09-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectorgroup-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cae09-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cae09-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectorgroup-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cae09-161">Java</span><span class="sxs-lookup"><span data-stu-id="cae09-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connectorgroup-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cae09-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="cae09-162">Response</span></span>
<span data-ttu-id="cae09-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cae09-163">The following is an example of the response.</span></span> <span data-ttu-id="cae09-164">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cae09-164">Note: The response object shown here might be shortened for readability.</span></span>
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



