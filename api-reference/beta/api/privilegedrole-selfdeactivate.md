---
title: 'privilegedRole: selfDeactivate'
description: Desative a função que é atribuída ao solicitante.
ms.openlocfilehash: f9f72a4f61dfd154829406eb535b394f8f137069
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033672"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="179f5-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="179f5-103">privilegedRole: selfDeactivate</span></span>

> <span data-ttu-id="179f5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="179f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="179f5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="179f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="179f5-106">Desative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="179f5-106">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="179f5-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="179f5-107">Permissions</span></span>
<span data-ttu-id="179f5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="179f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="179f5-110">O solicitante só pode chamar ```selfDeactivate``` para a função que é atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="179f5-110">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="179f5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="179f5-111">Permission type</span></span>      | <span data-ttu-id="179f5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="179f5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="179f5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="179f5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="179f5-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="179f5-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="179f5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="179f5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="179f5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="179f5-116">Not supported.</span></span>    |
|<span data-ttu-id="179f5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="179f5-117">Application</span></span> | <span data-ttu-id="179f5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="179f5-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="179f5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="179f5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="179f5-120">Observe que ``<id>`` é a id de função de destino.</span><span class="sxs-lookup"><span data-stu-id="179f5-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="179f5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="179f5-121">Request headers</span></span>
| <span data-ttu-id="179f5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="179f5-122">Name</span></span>       | <span data-ttu-id="179f5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="179f5-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="179f5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="179f5-124">Authorization</span></span>  | <span data-ttu-id="179f5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="179f5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="179f5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="179f5-127">Request body</span></span>
<span data-ttu-id="179f5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="179f5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="179f5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="179f5-129">Response</span></span>

<span data-ttu-id="179f5-130">Se tiver êxito, este método retornará `200 OK` objeto response de código e [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="179f5-130">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="179f5-131">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="179f5-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="179f5-132">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="179f5-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="179f5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="179f5-133">Example</span></span>
<span data-ttu-id="179f5-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="179f5-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="179f5-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="179f5-135">Request</span></span>
<span data-ttu-id="179f5-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="179f5-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="179f5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="179f5-137">Response</span></span>
<span data-ttu-id="179f5-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="179f5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->