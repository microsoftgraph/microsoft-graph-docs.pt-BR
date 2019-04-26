---
title: Obter grupos de membros
description: Retorna todos os grupos dos quais o usuário, grupo ou objeto de diretório especificado é membro. Esta função é transitiva.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c1d0bb1af8e88c125a0f4a672c431a21e1f5d9c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571965"
---
# <a name="get-member-groups"></a><span data-ttu-id="33439-104">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="33439-104">Get member groups</span></span>

<span data-ttu-id="33439-p102">Retorna todos os grupos dos quais o usuário, grupo ou objeto de diretório especificado é membro. Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="33439-p102">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="33439-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="33439-107">Permissions</span></span>
<span data-ttu-id="33439-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33439-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33439-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33439-110">Permission type</span></span>      | <span data-ttu-id="33439-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33439-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33439-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33439-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33439-113">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="33439-113">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="33439-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33439-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33439-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33439-115">Not supported.</span></span>    |
|<span data-ttu-id="33439-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33439-116">Application</span></span> | <span data-ttu-id="33439-117">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="33439-117">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33439-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33439-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="33439-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33439-119">Request headers</span></span>
| <span data-ttu-id="33439-120">Nome</span><span class="sxs-lookup"><span data-stu-id="33439-120">Name</span></span>       | <span data-ttu-id="33439-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="33439-121">Type</span></span> | <span data-ttu-id="33439-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="33439-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33439-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33439-123">Authorization</span></span>  | <span data-ttu-id="33439-124">string</span><span class="sxs-lookup"><span data-stu-id="33439-124">string</span></span>  | <span data-ttu-id="33439-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33439-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33439-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33439-127">Content-Type</span></span>   | <span data-ttu-id="33439-128">string</span><span class="sxs-lookup"><span data-stu-id="33439-128">string</span></span>  | <span data-ttu-id="33439-129">application/json</span><span class="sxs-lookup"><span data-stu-id="33439-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="33439-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33439-130">Request body</span></span>
<span data-ttu-id="33439-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33439-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="33439-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="33439-132">Parameter</span></span>    | <span data-ttu-id="33439-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="33439-133">Type</span></span>   |<span data-ttu-id="33439-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="33439-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33439-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="33439-135">securityEnabledOnly</span></span>|<span data-ttu-id="33439-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="33439-136">Boolean</span></span>| <span data-ttu-id="33439-p105">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="33439-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="33439-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="33439-139">Response</span></span>

<span data-ttu-id="33439-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33439-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33439-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33439-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="33439-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33439-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="33439-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="33439-143">Response</span></span>
<span data-ttu-id="33439-p106">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33439-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
