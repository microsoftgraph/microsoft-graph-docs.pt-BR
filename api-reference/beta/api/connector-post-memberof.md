---
title: Adicionar um conector para connectorGroup
description: Use essa API para adicionar um conector para um novo connectorGroup.
ms.openlocfilehash: 6dfc681f997953420811fbd7223a8c121934949e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036935"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="8fad4-103">Adicionar um conector para connectorGroup</span><span class="sxs-lookup"><span data-stu-id="8fad4-103">Add Connector to connectorGroup</span></span>

> <span data-ttu-id="8fad4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8fad4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fad4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8fad4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8fad4-106">Use essa API para adicionar um conector para um novo connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="8fad4-106">Use this API to add a connector to a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="8fad4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8fad4-107">Permissions</span></span>
<span data-ttu-id="8fad4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fad4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fad4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fad4-110">Permission type</span></span>      | <span data-ttu-id="8fad4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8fad4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fad4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fad4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8fad4-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8fad4-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8fad4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fad4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fad4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fad4-115">Not supported.</span></span>    |
|<span data-ttu-id="8fad4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fad4-116">Application</span></span> | <span data-ttu-id="8fad4-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fad4-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fad4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fad4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectors/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="8fad4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fad4-119">Request headers</span></span>
| <span data-ttu-id="8fad4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8fad4-120">Name</span></span>       | <span data-ttu-id="8fad4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fad4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8fad4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fad4-122">Authorization</span></span>  | <span data-ttu-id="8fad4-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="8fad4-123">Bearer.</span></span> <span data-ttu-id="8fad4-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8fad4-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fad4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fad4-125">Request body</span></span>
<span data-ttu-id="8fad4-126">No corpo da solicitação, fornece uma representação JSON do objeto [connectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="8fad4-126">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8fad4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fad4-127">Response</span></span>

<span data-ttu-id="8fad4-128">Se tiver êxito, este método retornará `201 Created` objeto response de código e [connectorGroup](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fad4-128">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fad4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fad4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8fad4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fad4-130">Request</span></span>
<span data-ttu-id="8fad4-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fad4-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connector"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectors/{id}/memberOf
Content-type: application/json
Content-length: 99

{
  "@odata.id": "https://graph.microsoft.com/{ver}/connectorGroups/{id}"
}
```
<span data-ttu-id="8fad4-132">No corpo da solicitação, fornece uma representação JSON do objeto [connectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="8fad4-132">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8fad4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fad4-133">Response</span></span>
<span data-ttu-id="8fad4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fad4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
