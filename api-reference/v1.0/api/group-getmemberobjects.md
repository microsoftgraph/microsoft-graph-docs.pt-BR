---
title: 'group: getMemberObjects'
description: 'Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.'
localization_priority: Normal
ms.openlocfilehash: fac39adebc8220458b3fcd0a46a5de5f6e27ab4a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891256"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="dcd08-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="dcd08-105">group: getMemberObjects</span></span>
<span data-ttu-id="dcd08-p102">Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.</span><span class="sxs-lookup"><span data-stu-id="dcd08-p102">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcd08-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcd08-109">Permissions</span></span>
<span data-ttu-id="dcd08-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcd08-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcd08-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcd08-112">Permission type</span></span>      | <span data-ttu-id="dcd08-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcd08-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcd08-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcd08-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dcd08-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dcd08-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dcd08-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcd08-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcd08-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcd08-117">Not supported.</span></span>    |
|<span data-ttu-id="dcd08-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcd08-118">Application</span></span> | <span data-ttu-id="dcd08-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcd08-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcd08-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcd08-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="dcd08-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd08-121">Request headers</span></span>
| <span data-ttu-id="dcd08-122">Nome</span><span class="sxs-lookup"><span data-stu-id="dcd08-122">Name</span></span>       | <span data-ttu-id="dcd08-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcd08-123">Type</span></span> | <span data-ttu-id="dcd08-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcd08-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dcd08-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcd08-125">Authorization</span></span>  | <span data-ttu-id="dcd08-126">string</span><span class="sxs-lookup"><span data-stu-id="dcd08-126">string</span></span>  | <span data-ttu-id="dcd08-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcd08-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcd08-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd08-129">Request body</span></span>
<span data-ttu-id="dcd08-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcd08-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dcd08-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dcd08-131">Parameter</span></span>    | <span data-ttu-id="dcd08-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcd08-132">Type</span></span>   |<span data-ttu-id="dcd08-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcd08-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcd08-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="dcd08-134">securityEnabledOnly</span></span>|<span data-ttu-id="dcd08-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="dcd08-135">Boolean</span></span>| <span data-ttu-id="dcd08-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="dcd08-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="dcd08-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcd08-138">Response</span></span>
<span data-ttu-id="dcd08-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="dcd08-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="dcd08-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcd08-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dcd08-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd08-141">Request</span></span>
<span data-ttu-id="dcd08-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcd08-142">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="dcd08-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcd08-143">Response</span></span>
<span data-ttu-id="dcd08-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcd08-144">The following is an example of the response.</span></span>
><span data-ttu-id="dcd08-145">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dcd08-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dcd08-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcd08-146">All the properties will be returned from an actual call.</span></span>
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
