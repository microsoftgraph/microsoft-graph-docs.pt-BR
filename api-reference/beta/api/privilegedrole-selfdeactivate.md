---
title: 'privilegedRole: selfDeactivate'
description: Desative a função que é atribuída ao solicitante.
localization_priority: Normal
ms.openlocfilehash: 4e627486cf58f1ea7bc71e29fe9c06c3fa3dfb25
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337410"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="a2af7-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="a2af7-103">privilegedRole: selfDeactivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2af7-104">Desative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="a2af7-104">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="a2af7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2af7-105">Permissions</span></span>
<span data-ttu-id="a2af7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2af7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a2af7-108">O solicitante só pode chamar ```selfDeactivate``` a função que é atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="a2af7-108">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="a2af7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2af7-109">Permission type</span></span>      | <span data-ttu-id="a2af7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2af7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2af7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2af7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a2af7-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a2af7-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a2af7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2af7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2af7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2af7-114">Not supported.</span></span>    |
|<span data-ttu-id="a2af7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2af7-115">Application</span></span> | <span data-ttu-id="a2af7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2af7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2af7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2af7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="a2af7-118">Observe que ``<id>`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="a2af7-118">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a2af7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2af7-119">Request headers</span></span>
| <span data-ttu-id="a2af7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a2af7-120">Name</span></span>       | <span data-ttu-id="a2af7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2af7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a2af7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2af7-122">Authorization</span></span>  | <span data-ttu-id="a2af7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2af7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2af7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2af7-125">Request body</span></span>
<span data-ttu-id="a2af7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2af7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2af7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2af7-127">Response</span></span>

<span data-ttu-id="a2af7-128">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2af7-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="a2af7-129">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="a2af7-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a2af7-130">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="a2af7-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="a2af7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2af7-131">Example</span></span>
<span data-ttu-id="a2af7-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a2af7-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a2af7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2af7-133">Request</span></span>
<span data-ttu-id="a2af7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2af7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="a2af7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2af7-135">Response</span></span>
<span data-ttu-id="a2af7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2af7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
