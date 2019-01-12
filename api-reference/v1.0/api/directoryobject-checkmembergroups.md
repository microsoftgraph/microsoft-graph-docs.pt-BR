---
title: Verificar grupos de membros
description: Verificar a associação em uma lista especificada de grupos e retorna a partir dessa lista desses grupos
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99ebf38b8f230233b50fa642f7503302afd02b33
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941783"
---
# <a name="check-member-groups"></a><span data-ttu-id="12e1e-103">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="12e1e-103">Check member groups</span></span>

<span data-ttu-id="12e1e-p101">Verifica se há associação em uma lista de grupos especificada e retorna dessa lista os grupos dos quais o usuário, grupo ou objeto de diretório especificado é membro. Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="12e1e-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="12e1e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="12e1e-106">Permissions</span></span>
<span data-ttu-id="12e1e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12e1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12e1e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12e1e-109">Permission type</span></span>      | <span data-ttu-id="12e1e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12e1e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12e1e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12e1e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="12e1e-112">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="12e1e-112">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="12e1e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12e1e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12e1e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12e1e-114">Not supported.</span></span>    |
|<span data-ttu-id="12e1e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12e1e-115">Application</span></span> | <span data-ttu-id="12e1e-116">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="12e1e-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12e1e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12e1e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="12e1e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12e1e-118">Request headers</span></span>
| <span data-ttu-id="12e1e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="12e1e-119">Name</span></span>       | <span data-ttu-id="12e1e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="12e1e-120">Type</span></span> | <span data-ttu-id="12e1e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="12e1e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12e1e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="12e1e-122">Authorization</span></span>  | <span data-ttu-id="12e1e-123">string</span><span class="sxs-lookup"><span data-stu-id="12e1e-123">string</span></span>  | <span data-ttu-id="12e1e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12e1e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12e1e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12e1e-126">Content-Type</span></span>  | <span data-ttu-id="12e1e-127">string</span><span class="sxs-lookup"><span data-stu-id="12e1e-127">string</span></span> | <span data-ttu-id="12e1e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="12e1e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12e1e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12e1e-129">Request body</span></span>
<span data-ttu-id="12e1e-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12e1e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="12e1e-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="12e1e-131">Parameter</span></span>    | <span data-ttu-id="12e1e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="12e1e-132">Type</span></span>   |<span data-ttu-id="12e1e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="12e1e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12e1e-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="12e1e-134">groupIds</span></span>|<span data-ttu-id="12e1e-135">String collection</span><span class="sxs-lookup"><span data-stu-id="12e1e-135">String collection</span></span>|<span data-ttu-id="12e1e-p104">Uma coleção que contém as IDs de objetos dos grupos em que se deve verificar a associação. Até 20 grupos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="12e1e-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="12e1e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="12e1e-138">Response</span></span>

<span data-ttu-id="12e1e-139">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12e1e-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12e1e-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12e1e-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="12e1e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12e1e-141">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="12e1e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="12e1e-142">Response</span></span>
<span data-ttu-id="12e1e-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12e1e-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
