---
title: Criar connectorGroup
description: Crie um objeto connectorGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 0d0954ebee00cfb3e979aa3fb39676f6b927f28f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130042"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="470e8-103">Criar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="470e8-103">Create connectorGroup</span></span>

<span data-ttu-id="470e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="470e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="470e8-105">Crie um [objeto connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="470e8-105">Create a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="470e8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="470e8-106">Permissions</span></span>
<span data-ttu-id="470e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="470e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="470e8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="470e8-109">Permission type</span></span>      | <span data-ttu-id="470e8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="470e8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="470e8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="470e8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="470e8-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="470e8-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="470e8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="470e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="470e8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="470e8-114">Not supported.</span></span>    |
|<span data-ttu-id="470e8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="470e8-115">Application</span></span> | <span data-ttu-id="470e8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="470e8-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="470e8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="470e8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-request-headers"></a><span data-ttu-id="470e8-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="470e8-118">Optional request headers</span></span>
| <span data-ttu-id="470e8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="470e8-119">Name</span></span>       | <span data-ttu-id="470e8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="470e8-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="470e8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="470e8-121">Authorization</span></span>  | <span data-ttu-id="470e8-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="470e8-122">Bearer.</span></span> <span data-ttu-id="470e8-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="470e8-123">Required.</span></span>|
| <span data-ttu-id="470e8-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="470e8-124">Content-type</span></span> | <span data-ttu-id="470e8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="470e8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="470e8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="470e8-127">Request body</span></span>
<span data-ttu-id="470e8-128">No corpo da solicitação, fornece uma representação JSON de um [objeto connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="470e8-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>
<span data-ttu-id="470e8-129">A tabela a seguir lista as propriedades disponíveis para um **connectorGroup**.</span><span class="sxs-lookup"><span data-stu-id="470e8-129">The following table lists the properties available for a **connectorGroup**.</span></span> <span data-ttu-id="470e8-130">A **propriedade** name é uma propriedade necessária.</span><span class="sxs-lookup"><span data-stu-id="470e8-130">The **name** property is a required property.</span></span>

| <span data-ttu-id="470e8-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="470e8-131">Property</span></span>     | <span data-ttu-id="470e8-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="470e8-132">Type</span></span>   |<span data-ttu-id="470e8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="470e8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="470e8-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="470e8-134">connectorGroupType</span></span>|<span data-ttu-id="470e8-135">string</span><span class="sxs-lookup"><span data-stu-id="470e8-135">string</span></span>| <span data-ttu-id="470e8-136">Indica o tipo de agente híbrido.</span><span class="sxs-lookup"><span data-stu-id="470e8-136">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="470e8-137">Essa propriedade é predefinida pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="470e8-137">This property is preset by the system.</span></span>|
|<span data-ttu-id="470e8-138">id</span><span class="sxs-lookup"><span data-stu-id="470e8-138">id</span></span>|<span data-ttu-id="470e8-139">string</span><span class="sxs-lookup"><span data-stu-id="470e8-139">string</span></span>| <span data-ttu-id="470e8-140">Identificador exclusivo deste connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="470e8-140">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="470e8-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="470e8-141">Read-only.</span></span> |
|<span data-ttu-id="470e8-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="470e8-142">isDefault</span></span>|<span data-ttu-id="470e8-143">booliano</span><span class="sxs-lookup"><span data-stu-id="470e8-143">boolean</span></span>| <span data-ttu-id="470e8-144">Indica se o connectorGroup é o padrão.</span><span class="sxs-lookup"><span data-stu-id="470e8-144">Indicates whether the connectorGroup is the default.</span></span> <span data-ttu-id="470e8-145">Somente um único grupo de conectores pode ser o connectorGroup padrão e isso é predefinido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="470e8-145">Only a single connector group can be the default connectorGroup and this is preset by the system.</span></span> |
|<span data-ttu-id="470e8-146">nome</span><span class="sxs-lookup"><span data-stu-id="470e8-146">name</span></span>|<span data-ttu-id="470e8-147">string</span><span class="sxs-lookup"><span data-stu-id="470e8-147">string</span></span>| <span data-ttu-id="470e8-148">O nome associado ao connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="470e8-148">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="470e8-149">region</span><span class="sxs-lookup"><span data-stu-id="470e8-149">region</span></span>|<span data-ttu-id="470e8-150">string</span><span class="sxs-lookup"><span data-stu-id="470e8-150">string</span></span>| <span data-ttu-id="470e8-151">A região à que o connectorGroup está atribuído e otimizará o tráfego.</span><span class="sxs-lookup"><span data-stu-id="470e8-151">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="470e8-152">Essa região só poderá ser definida se **nenhum** conector ou aplicativo estiver atribuído ao connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="470e8-152">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="470e8-153">As regiões disponíveis incluem: América do Norte, Europa, Austrália, Ásia e Índia.</span><span class="sxs-lookup"><span data-stu-id="470e8-153">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="470e8-154">Os valores possíveis são: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="470e8-154">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="470e8-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="470e8-155">Response</span></span>

<span data-ttu-id="470e8-156">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto connectorGroup](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="470e8-156">If successful, this method returns a `201 Created` response code and a [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="470e8-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="470e8-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="470e8-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="470e8-158">Request</span></span>
<span data-ttu-id="470e8-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="470e8-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="470e8-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="470e8-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "Connector Group Demo"

}
```
# <a name="c"></a>[<span data-ttu-id="470e8-161">C#</span><span class="sxs-lookup"><span data-stu-id="470e8-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="470e8-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="470e8-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="470e8-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="470e8-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="470e8-164">Java</span><span class="sxs-lookup"><span data-stu-id="470e8-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="470e8-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="470e8-165">Response</span></span>
<span data-ttu-id="470e8-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="470e8-166">The following is an example of the response.</span></span> 

><span data-ttu-id="470e8-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="470e8-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
  "name": "Connector Group Demo",
  "connectorGroupType": "applicationProxy",
  "isDefault": true,
  "region": "nam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



