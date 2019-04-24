---
title: Atualizar connectorGroups
description: Atualize as propriedades do objeto de conexão.
localization_priority: Normal
ms.openlocfilehash: 9d6feec19552aeeebe51ba0fab07e805c6f4a2bb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455762"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="0ffe9-103">Atualizar connectorGroups</span><span class="sxs-lookup"><span data-stu-id="0ffe9-103">Update connectorGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ffe9-104">Atualize as propriedades do objeto de conexão.</span><span class="sxs-lookup"><span data-stu-id="0ffe9-104">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ffe9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ffe9-105">Permissions</span></span>
<span data-ttu-id="0ffe9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ffe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ffe9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ffe9-108">Permission type</span></span>      | <span data-ttu-id="0ffe9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ffe9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ffe9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ffe9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ffe9-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ffe9-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0ffe9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ffe9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ffe9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ffe9-113">Not supported.</span></span>    |
|<span data-ttu-id="0ffe9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ffe9-114">Application</span></span> | <span data-ttu-id="0ffe9-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ffe9-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ffe9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ffe9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0ffe9-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0ffe9-117">Optional request headers</span></span>
| <span data-ttu-id="0ffe9-118">Name</span><span class="sxs-lookup"><span data-stu-id="0ffe9-118">Name</span></span>       | <span data-ttu-id="0ffe9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ffe9-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0ffe9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ffe9-120">Authorization</span></span>  | <span data-ttu-id="0ffe9-121">Portador.</span><span class="sxs-lookup"><span data-stu-id="0ffe9-121">Bearer.</span></span> <span data-ttu-id="0ffe9-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="0ffe9-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ffe9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ffe9-123">Request body</span></span>
<span data-ttu-id="0ffe9-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0ffe9-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0ffe9-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ffe9-127">Property</span></span>     | <span data-ttu-id="0ffe9-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ffe9-128">Type</span></span>   |<span data-ttu-id="0ffe9-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ffe9-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ffe9-130">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="0ffe9-130">connectorGroupType</span></span>|<span data-ttu-id="0ffe9-131">string</span><span class="sxs-lookup"><span data-stu-id="0ffe9-131">string</span></span>| <span data-ttu-id="0ffe9-132">Os valores possíveis são `applicationProxy`:.</span><span class="sxs-lookup"><span data-stu-id="0ffe9-132">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="0ffe9-133">nome</span><span class="sxs-lookup"><span data-stu-id="0ffe9-133">name</span></span>|<span data-ttu-id="0ffe9-134">String</span><span class="sxs-lookup"><span data-stu-id="0ffe9-134">String</span></span>|<span data-ttu-id="0ffe9-135">O nome do conector.</span><span class="sxs-lookup"><span data-stu-id="0ffe9-135">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="0ffe9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ffe9-136">Response</span></span>

<span data-ttu-id="0ffe9-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de teleconnector atualizado no corpo da resposta. [](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="0ffe9-137">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ffe9-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ffe9-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ffe9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ffe9-139">Request</span></span>
<span data-ttu-id="0ffe9-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ffe9-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0ffe9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ffe9-141">Response</span></span>
<span data-ttu-id="0ffe9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ffe9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
