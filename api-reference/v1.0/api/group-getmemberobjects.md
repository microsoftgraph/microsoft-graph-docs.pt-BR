---
title: 'group: getMemberObjects'
description: 'Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.'
ms.openlocfilehash: 59f3408434c77290552080b6b7b99a20e6fe19db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005561"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="d3465-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="d3465-105">group: getMemberObjects</span></span>
<span data-ttu-id="d3465-p102">Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.</span><span class="sxs-lookup"><span data-stu-id="d3465-p102">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3465-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3465-109">Permissions</span></span>
<span data-ttu-id="d3465-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3465-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3465-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3465-112">Permission type</span></span>      | <span data-ttu-id="d3465-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3465-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3465-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3465-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d3465-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d3465-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d3465-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3465-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3465-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3465-117">Not supported.</span></span>    |
|<span data-ttu-id="d3465-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3465-118">Application</span></span> | <span data-ttu-id="d3465-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3465-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3465-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3465-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="d3465-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3465-121">Request headers</span></span>
| <span data-ttu-id="d3465-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d3465-122">Name</span></span>       | <span data-ttu-id="d3465-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3465-123">Type</span></span> | <span data-ttu-id="d3465-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3465-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d3465-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3465-125">Authorization</span></span>  | <span data-ttu-id="d3465-126">string</span><span class="sxs-lookup"><span data-stu-id="d3465-126">string</span></span>  | <span data-ttu-id="d3465-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3465-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3465-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3465-129">Request body</span></span>
<span data-ttu-id="d3465-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3465-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d3465-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d3465-131">Parameter</span></span>    | <span data-ttu-id="d3465-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3465-132">Type</span></span>   |<span data-ttu-id="d3465-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3465-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3465-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="d3465-134">securityEnabledOnly</span></span>|<span data-ttu-id="d3465-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="d3465-135">Boolean</span></span>| <span data-ttu-id="d3465-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="d3465-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="d3465-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3465-138">Response</span></span>
<span data-ttu-id="d3465-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="d3465-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="d3465-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3465-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d3465-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3465-141">Request</span></span>
<span data-ttu-id="d3465-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3465-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="d3465-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3465-143">Response</span></span>
<span data-ttu-id="d3465-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3465-144">The following is an example of the response.</span></span>
><span data-ttu-id="d3465-145">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d3465-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d3465-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3465-146">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
