---
title: Criar um conector
description: Criar um objeto de conexão.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7978a526884d6d1c1c8c286a9ea9caa4f01f4302
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006856"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="b01c2-103">Criar um conector</span><span class="sxs-lookup"><span data-stu-id="b01c2-103">Create connectorGroup</span></span>

<span data-ttu-id="b01c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b01c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b01c2-105">Criar um objeto de [conexão](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="b01c2-105">Create a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b01c2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b01c2-106">Permissions</span></span>
<span data-ttu-id="b01c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b01c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b01c2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b01c2-109">Permission type</span></span>      | <span data-ttu-id="b01c2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b01c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b01c2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b01c2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b01c2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b01c2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b01c2-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b01c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b01c2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b01c2-114">Not supported.</span></span>    |
|<span data-ttu-id="b01c2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b01c2-115">Application</span></span> | <span data-ttu-id="b01c2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b01c2-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b01c2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b01c2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-request-headers"></a><span data-ttu-id="b01c2-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b01c2-118">Optional request headers</span></span>
| <span data-ttu-id="b01c2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b01c2-119">Name</span></span>       | <span data-ttu-id="b01c2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b01c2-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b01c2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b01c2-121">Authorization</span></span>  | <span data-ttu-id="b01c2-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="b01c2-122">Bearer.</span></span> <span data-ttu-id="b01c2-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b01c2-123">Required.</span></span>|
| <span data-ttu-id="b01c2-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="b01c2-124">Content-type</span></span> | <span data-ttu-id="b01c2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b01c2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b01c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b01c2-127">Request body</span></span>
<span data-ttu-id="b01c2-128">No corpo da solicitação, forneça uma representação JSON de um objeto do objeto de [conexão](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="b01c2-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>
<span data-ttu-id="b01c2-129">A tabela a seguir lista as propriedades disponíveis para um **conector**.</span><span class="sxs-lookup"><span data-stu-id="b01c2-129">The following table lists the properties available for a **connectorGroup**.</span></span> <span data-ttu-id="b01c2-130">A propriedade **Name** é uma propriedade necessária.</span><span class="sxs-lookup"><span data-stu-id="b01c2-130">The **name** property is a required property.</span></span>

| <span data-ttu-id="b01c2-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b01c2-131">Property</span></span>     | <span data-ttu-id="b01c2-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b01c2-132">Type</span></span>   |<span data-ttu-id="b01c2-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b01c2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b01c2-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="b01c2-134">connectorGroupType</span></span>|<span data-ttu-id="b01c2-135">string</span><span class="sxs-lookup"><span data-stu-id="b01c2-135">string</span></span>| <span data-ttu-id="b01c2-136">Indica o tipo de agente híbrido.</span><span class="sxs-lookup"><span data-stu-id="b01c2-136">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="b01c2-137">Esta propriedade é predefinida pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="b01c2-137">This property is preset by the system.</span></span>|
|<span data-ttu-id="b01c2-138">id</span><span class="sxs-lookup"><span data-stu-id="b01c2-138">id</span></span>|<span data-ttu-id="b01c2-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b01c2-139">string</span></span>| <span data-ttu-id="b01c2-140">Identificador exclusivo desse conector.</span><span class="sxs-lookup"><span data-stu-id="b01c2-140">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="b01c2-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b01c2-141">Read-only.</span></span> |
|<span data-ttu-id="b01c2-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="b01c2-142">isDefault</span></span>|<span data-ttu-id="b01c2-143">booliano</span><span class="sxs-lookup"><span data-stu-id="b01c2-143">boolean</span></span>| <span data-ttu-id="b01c2-144">Indica se o conector é o padrão.</span><span class="sxs-lookup"><span data-stu-id="b01c2-144">Indicates whether the connectorGroup is the default.</span></span> <span data-ttu-id="b01c2-145">Somente um grupo de conectores único pode ser o grupo de conectores padrão e é predefinido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="b01c2-145">Only a single connector group can be the default connectorGroup and this is preset by the system.</span></span> |
|<span data-ttu-id="b01c2-146">nome</span><span class="sxs-lookup"><span data-stu-id="b01c2-146">name</span></span>|<span data-ttu-id="b01c2-147">string</span><span class="sxs-lookup"><span data-stu-id="b01c2-147">string</span></span>| <span data-ttu-id="b01c2-148">O nome associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="b01c2-148">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="b01c2-149">região</span><span class="sxs-lookup"><span data-stu-id="b01c2-149">region</span></span>|<span data-ttu-id="b01c2-150">string</span><span class="sxs-lookup"><span data-stu-id="b01c2-150">string</span></span>| <span data-ttu-id="b01c2-151">A região à qual o conector é atribuído e otimizará o tráfego para o.</span><span class="sxs-lookup"><span data-stu-id="b01c2-151">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="b01c2-152">Essa região só poderá ser definida se **nenhum** conector ou aplicativo for atribuído ao grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="b01c2-152">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="b01c2-153">As regiões disponíveis incluem: América do Norte, Europa, Austrália, Ásia e Índia.</span><span class="sxs-lookup"><span data-stu-id="b01c2-153">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="b01c2-154">Os valores possíveis são: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="b01c2-154">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="b01c2-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b01c2-155">Response</span></span>

<span data-ttu-id="b01c2-156">Se tiver êxito, este método retornará um `201 Created` código de resposta [connectorGroup](../resources/connectorgroup.md) e um objeto de um, no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b01c2-156">If successful, this method returns a `201 Created` response code and a [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b01c2-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b01c2-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="b01c2-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b01c2-158">Request</span></span>
<span data-ttu-id="b01c2-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b01c2-159">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b01c2-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="b01c2-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b01c2-161">C#</span><span class="sxs-lookup"><span data-stu-id="b01c2-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b01c2-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b01c2-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b01c2-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b01c2-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b01c2-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="b01c2-164">Response</span></span>
<span data-ttu-id="b01c2-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b01c2-165">The following is an example of the response.</span></span> 

><span data-ttu-id="b01c2-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b01c2-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
