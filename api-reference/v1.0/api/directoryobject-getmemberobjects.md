---
title: Obter objetos de membros
description: " Retorna todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. Esta função é transitiva. "
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 03d70d0b26746f42f920daf3666ca37db5f1e15b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578642"
---
# <a name="get-member-objects"></a><span data-ttu-id="83298-104">Obter objetos de membros</span><span class="sxs-lookup"><span data-stu-id="83298-104">Get member objects</span></span>

 <span data-ttu-id="83298-p102">Retorna todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="83298-p102">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="83298-107">Observação: Somente usuários podem ser membros de funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="83298-107">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="83298-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="83298-108">Permissions</span></span>
<span data-ttu-id="83298-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83298-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83298-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83298-111">Permission type</span></span>      | <span data-ttu-id="83298-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83298-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83298-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83298-113">Delegated (work or school account)</span></span> | <span data-ttu-id="83298-114">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="83298-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="83298-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83298-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83298-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83298-116">Not supported.</span></span>    |
|<span data-ttu-id="83298-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83298-117">Application</span></span> | <span data-ttu-id="83298-118">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="83298-118">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83298-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83298-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="83298-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83298-120">Request headers</span></span>
| <span data-ttu-id="83298-121">Nome</span><span class="sxs-lookup"><span data-stu-id="83298-121">Name</span></span>       | <span data-ttu-id="83298-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="83298-122">Type</span></span> | <span data-ttu-id="83298-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="83298-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="83298-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="83298-124">Authorization</span></span>  | <span data-ttu-id="83298-125">string</span><span class="sxs-lookup"><span data-stu-id="83298-125">string</span></span>  | <span data-ttu-id="83298-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83298-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83298-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83298-128">Content-Type</span></span>   | <span data-ttu-id="83298-129">string</span><span class="sxs-lookup"><span data-stu-id="83298-129">string</span></span>  | <span data-ttu-id="83298-130">application/json</span><span class="sxs-lookup"><span data-stu-id="83298-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83298-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83298-131">Request body</span></span>
<span data-ttu-id="83298-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83298-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="83298-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="83298-133">Parameter</span></span>    | <span data-ttu-id="83298-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="83298-134">Type</span></span>   |<span data-ttu-id="83298-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="83298-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83298-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="83298-136">securityEnabledOnly</span></span>|<span data-ttu-id="83298-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="83298-137">Boolean</span></span>| <span data-ttu-id="83298-p105">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="83298-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="83298-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="83298-140">Response</span></span>

<span data-ttu-id="83298-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83298-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83298-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83298-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="83298-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83298-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="83298-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="83298-144">Response</span></span>
<span data-ttu-id="83298-p106">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83298-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
