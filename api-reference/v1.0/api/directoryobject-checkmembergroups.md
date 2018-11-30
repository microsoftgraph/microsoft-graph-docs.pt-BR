---
title: Verificar grupos de membros
description: Verificar a associação em uma lista especificada de grupos e retorna a partir dessa lista desses grupos
ms.openlocfilehash: 174531d11944a98c31d56b113a3221b75bac18e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005767"
---
# <a name="check-member-groups"></a><span data-ttu-id="d47b0-103">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="d47b0-103">Check member groups</span></span>

<span data-ttu-id="d47b0-p101">Verifica se há associação em uma lista de grupos especificada e retorna dessa lista os grupos dos quais o usuário, grupo ou objeto de diretório especificado é membro. Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="d47b0-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="d47b0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d47b0-106">Permissions</span></span>
<span data-ttu-id="d47b0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d47b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d47b0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d47b0-109">Permission type</span></span>      | <span data-ttu-id="d47b0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d47b0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d47b0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d47b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d47b0-112">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47b0-112">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="d47b0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d47b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d47b0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d47b0-114">Not supported.</span></span>    |
|<span data-ttu-id="d47b0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d47b0-115">Application</span></span> | <span data-ttu-id="d47b0-116">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47b0-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d47b0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d47b0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="d47b0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d47b0-118">Request headers</span></span>
| <span data-ttu-id="d47b0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d47b0-119">Name</span></span>       | <span data-ttu-id="d47b0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d47b0-120">Type</span></span> | <span data-ttu-id="d47b0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d47b0-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d47b0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d47b0-122">Authorization</span></span>  | <span data-ttu-id="d47b0-123">string</span><span class="sxs-lookup"><span data-stu-id="d47b0-123">string</span></span>  | <span data-ttu-id="d47b0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d47b0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d47b0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d47b0-126">Content-Type</span></span>  | <span data-ttu-id="d47b0-127">string</span><span class="sxs-lookup"><span data-stu-id="d47b0-127">string</span></span> | <span data-ttu-id="d47b0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d47b0-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d47b0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d47b0-129">Request body</span></span>
<span data-ttu-id="d47b0-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d47b0-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d47b0-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d47b0-131">Parameter</span></span>    | <span data-ttu-id="d47b0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d47b0-132">Type</span></span>   |<span data-ttu-id="d47b0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d47b0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d47b0-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="d47b0-134">groupIds</span></span>|<span data-ttu-id="d47b0-135">String collection</span><span class="sxs-lookup"><span data-stu-id="d47b0-135">String collection</span></span>|<span data-ttu-id="d47b0-p104">Uma coleção que contém as IDs de objetos dos grupos em que se deve verificar a associação. Até 20 grupos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="d47b0-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="d47b0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d47b0-138">Response</span></span>

<span data-ttu-id="d47b0-139">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d47b0-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d47b0-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d47b0-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d47b0-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d47b0-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="d47b0-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d47b0-142">Response</span></span>
<span data-ttu-id="d47b0-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d47b0-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
