---
title: 'group: getMemberObjects'
description: 'Retorne todos os grupos e unidades administrativas que o grupo é um membro de. A seleção é transitiva. Observação: Grupos não podem ser membros das funções de diretório, portanto nenhuma função de diretório será retornada.'
ms.openlocfilehash: e0ff719b58f13f036cbf8502725fb1e146cb1227
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036527"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="bb4e3-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="bb4e3-105">group: getMemberObjects</span></span>

> <span data-ttu-id="bb4e3-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb4e3-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb4e3-108">Retorne todos os grupos e unidades administrativas que o grupo é um membro de.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-108">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="bb4e3-109">A seleção é transitiva.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-109">The check is transitive.</span></span> <span data-ttu-id="bb4e3-110">Observação: Grupos não podem ser membros das funções de diretório, portanto nenhuma função de diretório será retornada.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-110">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb4e3-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="bb4e3-111">Permissions</span></span>
<span data-ttu-id="bb4e3-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb4e3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb4e3-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb4e3-114">Permission type</span></span>      | <span data-ttu-id="bb4e3-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb4e3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb4e3-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb4e3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="bb4e3-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb4e3-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bb4e3-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb4e3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb4e3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-119">Not supported.</span></span>    |
|<span data-ttu-id="bb4e3-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb4e3-120">Application</span></span> | <span data-ttu-id="bb4e3-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb4e3-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb4e3-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb4e3-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="bb4e3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb4e3-123">Request headers</span></span>
| <span data-ttu-id="bb4e3-124">Nome</span><span class="sxs-lookup"><span data-stu-id="bb4e3-124">Name</span></span>       | <span data-ttu-id="bb4e3-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb4e3-125">Type</span></span> | <span data-ttu-id="bb4e3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb4e3-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bb4e3-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb4e3-127">Authorization</span></span>  | <span data-ttu-id="bb4e3-128">string</span><span class="sxs-lookup"><span data-stu-id="bb4e3-128">string</span></span>  | <span data-ttu-id="bb4e3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb4e3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb4e3-131">Request body</span></span>
<span data-ttu-id="bb4e3-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bb4e3-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bb4e3-133">Parameter</span></span>    | <span data-ttu-id="bb4e3-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb4e3-134">Type</span></span>   |<span data-ttu-id="bb4e3-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb4e3-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb4e3-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="bb4e3-136">securityEnabledOnly</span></span>|<span data-ttu-id="bb4e3-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb4e3-137">Boolean</span></span>|<span data-ttu-id="bb4e3-p106">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="bb4e3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb4e3-140">Response</span></span>
<span data-ttu-id="bb4e3-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="bb4e3-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb4e3-142">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bb4e3-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb4e3-143">Request</span></span>
<span data-ttu-id="bb4e3-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="bb4e3-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb4e3-145">Response</span></span>
<span data-ttu-id="bb4e3-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-146">The following is an example of the response.</span></span>
><span data-ttu-id="bb4e3-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb4e3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
