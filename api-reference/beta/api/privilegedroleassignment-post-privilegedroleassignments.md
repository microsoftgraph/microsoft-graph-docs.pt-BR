---
title: Criar privilegedRoleAssignment
description: Use essa API para criar um novo privilegedRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 5522956b129eae8a19fd00b0e70b41380dbdd25e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513400"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="38762-103">Criar privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="38762-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38762-104">Use essa API para criar um novo [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="38762-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="38762-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="38762-105">Permissions</span></span>
<span data-ttu-id="38762-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38762-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="38762-108">O solicitante precisa ter a função de _Administrador com privilégios de função_ .</span><span class="sxs-lookup"><span data-stu-id="38762-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="38762-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38762-109">Permission type</span></span>      | <span data-ttu-id="38762-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38762-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38762-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38762-111">Delegated (work or school account)</span></span> | <span data-ttu-id="38762-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="38762-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="38762-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38762-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38762-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38762-114">Not supported.</span></span>    |
|<span data-ttu-id="38762-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38762-115">Application</span></span> | <span data-ttu-id="38762-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38762-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38762-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38762-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="38762-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38762-118">Request headers</span></span>
| <span data-ttu-id="38762-119">Nome</span><span class="sxs-lookup"><span data-stu-id="38762-119">Name</span></span>       | <span data-ttu-id="38762-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="38762-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="38762-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="38762-121">Authorization</span></span>  | <span data-ttu-id="38762-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38762-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38762-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38762-124">Request body</span></span>
<span data-ttu-id="38762-125">No corpo da solicitação, fornece uma representação JSON do objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="38762-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="38762-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="38762-126">Response</span></span>

<span data-ttu-id="38762-127">Se tiver êxito, este método retornará `201 Created` objeto response de código e [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38762-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="38762-128">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="38762-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="38762-129">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="38762-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="38762-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38762-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38762-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38762-131">Request</span></span>
<span data-ttu-id="38762-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38762-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
<span data-ttu-id="38762-133">No corpo da solicitação, fornece uma representação JSON do objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="38762-133">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="38762-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="38762-134">Response</span></span>
<span data-ttu-id="38762-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38762-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
