---
title: Atualizar connectorGroups
description: Atualize as propriedades do objeto de conexão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: ad83631d6707e5f72f0813a71f7e40497e1903b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437172"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="e5a93-103">Atualizar connectorGroups</span><span class="sxs-lookup"><span data-stu-id="e5a93-103">Update connectorGroups</span></span>

<span data-ttu-id="e5a93-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e5a93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5a93-105">Atualize as propriedades do objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="e5a93-105">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5a93-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5a93-106">Permissions</span></span>
<span data-ttu-id="e5a93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5a93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5a93-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5a93-109">Permission type</span></span>      | <span data-ttu-id="e5a93-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5a93-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5a93-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5a93-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e5a93-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5a93-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5a93-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5a93-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5a93-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5a93-114">Not supported.</span></span>    |
|<span data-ttu-id="e5a93-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5a93-115">Application</span></span> | <span data-ttu-id="e5a93-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5a93-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5a93-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5a93-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e5a93-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e5a93-118">Optional request headers</span></span>
| <span data-ttu-id="e5a93-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e5a93-119">Name</span></span>       | <span data-ttu-id="e5a93-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5a93-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e5a93-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5a93-121">Authorization</span></span>  | <span data-ttu-id="e5a93-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="e5a93-122">Bearer.</span></span> <span data-ttu-id="e5a93-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="e5a93-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5a93-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5a93-124">Request body</span></span>
<span data-ttu-id="e5a93-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e5a93-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e5a93-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5a93-128">Property</span></span>     | <span data-ttu-id="e5a93-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5a93-129">Type</span></span>   |<span data-ttu-id="e5a93-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5a93-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5a93-131">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="e5a93-131">connectorGroupType</span></span>|<span data-ttu-id="e5a93-132">string</span><span class="sxs-lookup"><span data-stu-id="e5a93-132">string</span></span>| <span data-ttu-id="e5a93-133">Os valores possíveis são `applicationProxy`:.</span><span class="sxs-lookup"><span data-stu-id="e5a93-133">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="e5a93-134">nome</span><span class="sxs-lookup"><span data-stu-id="e5a93-134">name</span></span>|<span data-ttu-id="e5a93-135">String</span><span class="sxs-lookup"><span data-stu-id="e5a93-135">String</span></span>|<span data-ttu-id="e5a93-136">O nome do conector.</span><span class="sxs-lookup"><span data-stu-id="e5a93-136">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="e5a93-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5a93-137">Response</span></span>

<span data-ttu-id="e5a93-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de [teleconnector](../resources/connectorgroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5a93-138">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5a93-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5a93-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5a93-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5a93-140">Request</span></span>
<span data-ttu-id="e5a93-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5a93-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
PATCH https://graph.microsoft.com/{ver}/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
}
```
##### <a name="response"></a><span data-ttu-id="e5a93-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5a93-142">Response</span></span>
<span data-ttu-id="e5a93-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5a93-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "isDefault": true
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
