---
title: Criar privilegedRoleAssignment
description: Use essa API para criar um novo privilegedRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 7957aa964361890572de11c375753a49a3a9e9e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852210"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="383da-103">Criar privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="383da-103">Create privilegedRoleAssignment</span></span>

> <span data-ttu-id="383da-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="383da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="383da-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="383da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="383da-106">Use essa API para criar um novo [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="383da-106">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="383da-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="383da-107">Permissions</span></span>
<span data-ttu-id="383da-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="383da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="383da-110">O solicitante precisa ter a função de _Administrador com privilégios de função_ .</span><span class="sxs-lookup"><span data-stu-id="383da-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="383da-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="383da-111">Permission type</span></span>      | <span data-ttu-id="383da-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="383da-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="383da-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="383da-113">Delegated (work or school account)</span></span> | <span data-ttu-id="383da-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="383da-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="383da-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="383da-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="383da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="383da-116">Not supported.</span></span>    |
|<span data-ttu-id="383da-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="383da-117">Application</span></span> | <span data-ttu-id="383da-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="383da-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="383da-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="383da-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="383da-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="383da-120">Request headers</span></span>
| <span data-ttu-id="383da-121">Nome</span><span class="sxs-lookup"><span data-stu-id="383da-121">Name</span></span>       | <span data-ttu-id="383da-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="383da-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="383da-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="383da-123">Authorization</span></span>  | <span data-ttu-id="383da-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="383da-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="383da-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="383da-126">Request body</span></span>
<span data-ttu-id="383da-127">No corpo da solicitação, fornece uma representação JSON do objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="383da-127">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="383da-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="383da-128">Response</span></span>

<span data-ttu-id="383da-129">Se tiver êxito, este método retornará `201 Created` objeto response de código e [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="383da-129">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="383da-130">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="383da-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="383da-131">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="383da-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="383da-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="383da-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="383da-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="383da-133">Request</span></span>
<span data-ttu-id="383da-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="383da-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="383da-135">No corpo da solicitação, fornece uma representação JSON do objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="383da-135">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="383da-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="383da-136">Response</span></span>
<span data-ttu-id="383da-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="383da-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
