---
title: Atualizar connectorGroups
description: Atualize as propriedades do objeto connectorgroup.
ms.openlocfilehash: a9777394a3ecfc65a7c03c07643359ef3c763aca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033370"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="5bdf7-103">Atualizar connectorGroups</span><span class="sxs-lookup"><span data-stu-id="5bdf7-103">Update connectorGroups</span></span>

> <span data-ttu-id="5bdf7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5bdf7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bdf7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5bdf7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5bdf7-106">Atualize as propriedades do objeto connectorgroup.</span><span class="sxs-lookup"><span data-stu-id="5bdf7-106">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5bdf7-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="5bdf7-107">Permissions</span></span>
<span data-ttu-id="5bdf7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bdf7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bdf7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bdf7-110">Permission type</span></span>      | <span data-ttu-id="5bdf7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bdf7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bdf7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bdf7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5bdf7-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5bdf7-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5bdf7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bdf7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bdf7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bdf7-115">Not supported.</span></span>    |
|<span data-ttu-id="5bdf7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bdf7-116">Application</span></span> | <span data-ttu-id="5bdf7-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bdf7-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bdf7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bdf7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="5bdf7-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="5bdf7-119">Optional request headers</span></span>
| <span data-ttu-id="5bdf7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5bdf7-120">Name</span></span>       | <span data-ttu-id="5bdf7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bdf7-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5bdf7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bdf7-122">Authorization</span></span>  | <span data-ttu-id="5bdf7-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="5bdf7-123">Bearer.</span></span> <span data-ttu-id="5bdf7-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="5bdf7-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bdf7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bdf7-125">Request body</span></span>
<span data-ttu-id="5bdf7-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5bdf7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5bdf7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bdf7-129">Property</span></span>     | <span data-ttu-id="5bdf7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bdf7-130">Type</span></span>   |<span data-ttu-id="5bdf7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bdf7-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bdf7-132">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="5bdf7-132">connectorGroupType</span></span>|<span data-ttu-id="5bdf7-133">string</span><span class="sxs-lookup"><span data-stu-id="5bdf7-133">string</span></span>| <span data-ttu-id="5bdf7-134">Os valores possíveis são: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="5bdf7-134">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="5bdf7-135">name</span><span class="sxs-lookup"><span data-stu-id="5bdf7-135">name</span></span>|<span data-ttu-id="5bdf7-136">String</span><span class="sxs-lookup"><span data-stu-id="5bdf7-136">String</span></span>|<span data-ttu-id="5bdf7-137">O nome da connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="5bdf7-137">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="5bdf7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bdf7-138">Response</span></span>

<span data-ttu-id="5bdf7-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [connectorGroup](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bdf7-139">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5bdf7-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bdf7-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bdf7-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bdf7-141">Request</span></span>
<span data-ttu-id="5bdf7-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bdf7-142">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5bdf7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bdf7-143">Response</span></span>
<span data-ttu-id="5bdf7-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5bdf7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
