---
title: Atualizar connectorGroups
description: Atualize as propriedades do objeto de conexão.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 80565045fa292b09e5c8e98544c466ec784f24f0
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44555792"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="b2404-103">Atualizar connectorGroups</span><span class="sxs-lookup"><span data-stu-id="b2404-103">Update connectorGroups</span></span>

<span data-ttu-id="b2404-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2404-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2404-105">Atualizar as propriedades de um objeto de [conexão](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="b2404-105">Update the properties of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2404-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2404-106">Permissions</span></span>
<span data-ttu-id="b2404-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2404-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2404-109">Permission type</span></span>      | <span data-ttu-id="b2404-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2404-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2404-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2404-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b2404-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b2404-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b2404-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2404-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2404-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2404-114">Not supported.</span></span>    |
|<span data-ttu-id="b2404-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2404-115">Application</span></span> | <span data-ttu-id="b2404-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2404-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2404-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2404-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b2404-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b2404-118">Optional request headers</span></span>
| <span data-ttu-id="b2404-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b2404-119">Name</span></span>       | <span data-ttu-id="b2404-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2404-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b2404-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2404-121">Authorization</span></span>  | <span data-ttu-id="b2404-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="b2404-122">Bearer.</span></span> <span data-ttu-id="b2404-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="b2404-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2404-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2404-124">Request body</span></span>
<span data-ttu-id="b2404-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b2404-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b2404-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2404-128">Property</span></span>     | <span data-ttu-id="b2404-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2404-129">Type</span></span>   |<span data-ttu-id="b2404-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2404-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2404-131">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="b2404-131">connectorGroupType</span></span>|<span data-ttu-id="b2404-132">string</span><span class="sxs-lookup"><span data-stu-id="b2404-132">string</span></span>| <span data-ttu-id="b2404-133">Indica o tipo de agente híbrido.</span><span class="sxs-lookup"><span data-stu-id="b2404-133">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="b2404-134">Isso é definido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="b2404-134">This pre-set by the system.</span></span> |
|<span data-ttu-id="b2404-135">id</span><span class="sxs-lookup"><span data-stu-id="b2404-135">id</span></span>|<span data-ttu-id="b2404-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2404-136">string</span></span>| <span data-ttu-id="b2404-137">Identificador exclusivo desse conector.</span><span class="sxs-lookup"><span data-stu-id="b2404-137">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="b2404-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2404-138">Read-only.</span></span> |
|<span data-ttu-id="b2404-139">isDefault</span><span class="sxs-lookup"><span data-stu-id="b2404-139">isDefault</span></span>|<span data-ttu-id="b2404-140">booliano</span><span class="sxs-lookup"><span data-stu-id="b2404-140">boolean</span></span>| <span data-ttu-id="b2404-141">Indica se o conector de conexão é o padrão.</span><span class="sxs-lookup"><span data-stu-id="b2404-141">Indicates if the connectorGroup is the default connectorGroup.</span></span> <span data-ttu-id="b2404-142">Somente um grupo de conectores único pode ser o grupo de conectores padrão e é predefinido pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="b2404-142">Only a single connector group can be the default connectorGroup and this is pre-set by the system.</span></span> |
|<span data-ttu-id="b2404-143">nome</span><span class="sxs-lookup"><span data-stu-id="b2404-143">name</span></span>|<span data-ttu-id="b2404-144">string</span><span class="sxs-lookup"><span data-stu-id="b2404-144">string</span></span>| <span data-ttu-id="b2404-145">O nome associado ao conector.</span><span class="sxs-lookup"><span data-stu-id="b2404-145">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="b2404-146">região</span><span class="sxs-lookup"><span data-stu-id="b2404-146">region</span></span>|<span data-ttu-id="b2404-147">string</span><span class="sxs-lookup"><span data-stu-id="b2404-147">string</span></span>| <span data-ttu-id="b2404-148">A região à qual o conector é atribuído e otimizará o tráfego para o.</span><span class="sxs-lookup"><span data-stu-id="b2404-148">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="b2404-149">Essa região só poderá ser definida se **nenhum** conector ou aplicativo for atribuído ao grupo de conectores.</span><span class="sxs-lookup"><span data-stu-id="b2404-149">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="b2404-150">As regiões disponíveis incluem: América do Norte, Europa, Austrália, Ásia e Índia.</span><span class="sxs-lookup"><span data-stu-id="b2404-150">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="b2404-151">Os valores possíveis são: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="b2404-151">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="b2404-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2404-152">Response</span></span>

<span data-ttu-id="b2404-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [teleconnector](../resources/connectorgroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2404-153">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b2404-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2404-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2404-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2404-155">Request</span></span>
<span data-ttu-id="b2404-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2404-156">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b2404-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2404-157">Response</span></span>
<span data-ttu-id="b2404-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2404-158">The following is an example of the response.</span></span> <span data-ttu-id="b2404-159">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="b2404-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b2404-160">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2404-160">All of the properties will be returned from an actual call.</span></span>
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
