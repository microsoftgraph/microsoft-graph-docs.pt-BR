---
title: Criar um conector
description: Criar um objeto de conexão.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ddc1aebfeb64e4dd596f94dd8a91f3718a29fb7
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863260"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="63ea1-103">Criar um conector</span><span class="sxs-lookup"><span data-stu-id="63ea1-103">Create connectorGroup</span></span>

<span data-ttu-id="63ea1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63ea1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63ea1-105">Criar um objeto de [conexão](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="63ea1-105">Create a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="63ea1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="63ea1-106">Permissions</span></span>
<span data-ttu-id="63ea1-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="63ea1-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="63ea1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63ea1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63ea1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63ea1-109">Permission type</span></span>      | <span data-ttu-id="63ea1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63ea1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63ea1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63ea1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63ea1-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="63ea1-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="63ea1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63ea1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63ea1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63ea1-114">Not supported.</span></span>    |
|<span data-ttu-id="63ea1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63ea1-115">Application</span></span> | <span data-ttu-id="63ea1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63ea1-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="63ea1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63ea1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-request-headers"></a><span data-ttu-id="63ea1-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="63ea1-118">Optional request headers</span></span>
| <span data-ttu-id="63ea1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="63ea1-119">Name</span></span>       | <span data-ttu-id="63ea1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="63ea1-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="63ea1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="63ea1-121">Authorization</span></span>  | <span data-ttu-id="63ea1-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="63ea1-122">Bearer.</span></span> <span data-ttu-id="63ea1-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63ea1-123">Required.</span></span>|
| <span data-ttu-id="63ea1-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="63ea1-124">Content-type</span></span> | <span data-ttu-id="63ea1-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="63ea1-125">application/json.</span></span> <span data-ttu-id="63ea1-126">Required.</span><span class="sxs-lookup"><span data-stu-id="63ea1-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63ea1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63ea1-127">Request body</span></span>
<span data-ttu-id="63ea1-128">No corpo da solicitação, forneça uma representação JSON de um objeto do objeto de [conexão](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="63ea1-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>
<span data-ttu-id="63ea1-129">A tabela a seguir lista as propriedades disponíveis para um **conector**.</span><span class="sxs-lookup"><span data-stu-id="63ea1-129">The following table lists the properties available for a **connectorGroup**.</span></span> <span data-ttu-id="63ea1-130">A propriedade **Name** é uma propriedade necessária.</span><span class="sxs-lookup"><span data-stu-id="63ea1-130">The **name** property is a required property.</span></span>

| <span data-ttu-id="63ea1-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63ea1-131">Property</span></span>     | <span data-ttu-id="63ea1-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="63ea1-132">Type</span></span>   |<span data-ttu-id="63ea1-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="63ea1-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63ea1-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="63ea1-134">connectorGroupType</span></span>|<span data-ttu-id="63ea1-135">string</span><span class="sxs-lookup"><span data-stu-id="63ea1-135">string</span></span>| <span data-ttu-id="63ea1-136">Indica o tipo de agente híbrido.</span><span class="sxs-lookup"><span data-stu-id="63ea1-136">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="63ea1-137">Esta propriedade é predefinida pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="63ea1-137">This property is preset by the system.</span></span>|
|<span data-ttu-id="63ea1-138">id</span><span class="sxs-lookup"><span data-stu-id="63ea1-138">id</span></span>|<span data-ttu-id="63ea1-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63ea1-139">string</span></span>| <span data-ttu-id="63ea1-140">Identificador exclusivo desse conector.</span><span class="sxs-lookup"><span data-stu-id="63ea1-140">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="63ea1-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="63ea1-141">Read-only.</span></span> |
|<span data-ttu-id="63ea1-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="63ea1-142">isDefault</span></span>|<span data-ttu-id="63ea1-143">booliano</span><span class="sxs-lookup"><span data-stu-id="63ea1-143">boolean</span></span>| <span data-ttu-id="63ea1-144">Indica se o conector é o padrão.</span><span class="sxs-lookup"><span data-stu-id="63ea1-144">Indicates whether the connectorGroup is the default.</span></span> <span data-ttu-id="63ea1-145">Somente um grupo de conectores único pode ser o grupo de conectores padrão e é predefinido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="63ea1-145">Only a single connector group can be the default connectorGroup and this is preset by the system.</span></span> |
|<span data-ttu-id="63ea1-146">nome</span><span class="sxs-lookup"><span data-stu-id="63ea1-146">name</span></span>|<span data-ttu-id="63ea1-147">string</span><span class="sxs-lookup"><span data-stu-id="63ea1-147">string</span></span>| <span data-ttu-id="63ea1-148">O nome associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="63ea1-148">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="63ea1-149">região</span><span class="sxs-lookup"><span data-stu-id="63ea1-149">region</span></span>|<span data-ttu-id="63ea1-150">string</span><span class="sxs-lookup"><span data-stu-id="63ea1-150">string</span></span>| <span data-ttu-id="63ea1-151">A região à qual o conector é atribuído e otimizará o tráfego para o.</span><span class="sxs-lookup"><span data-stu-id="63ea1-151">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="63ea1-152">Essa região só poderá ser definida se **nenhum** conector ou aplicativo for atribuído ao grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="63ea1-152">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="63ea1-153">As regiões disponíveis incluem: América do Norte, Europa, Austrália, Ásia e Índia.</span><span class="sxs-lookup"><span data-stu-id="63ea1-153">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="63ea1-154">Os valores possíveis são: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="63ea1-154">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="63ea1-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="63ea1-155">Response</span></span>

<span data-ttu-id="63ea1-156">Se tiver êxito, este método retornará um `201 Created` código de resposta [connectorGroup](../resources/connectorgroup.md) e um objeto de um, no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63ea1-156">If successful, this method returns a `201 Created` response code and a [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="63ea1-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63ea1-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="63ea1-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63ea1-158">Request</span></span>
<span data-ttu-id="63ea1-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="63ea1-159">The following is an example of the request.</span></span>
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
### <a name="response"></a><span data-ttu-id="63ea1-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="63ea1-160">Response</span></span>
<span data-ttu-id="63ea1-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="63ea1-161">The following is an example of the response.</span></span> 

><span data-ttu-id="63ea1-162">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="63ea1-162">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="63ea1-163">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="63ea1-163">All the properties will be returned from an actual call.</span></span>
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
