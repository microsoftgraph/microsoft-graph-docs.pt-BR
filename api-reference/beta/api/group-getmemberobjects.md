---
title: 'group: getMemberObjects'
description: 'Retorne todos os grupos e unidades administrativas que o grupo é um membro de. A seleção é transitiva. Observação: Grupos não podem ser membros das funções de diretório, portanto nenhuma função de diretório será retornada.'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: a83987a15f384cf17e268a8bdbd6791164484f7e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935924"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="ec81a-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="ec81a-105">group: getMemberObjects</span></span>

> <span data-ttu-id="ec81a-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ec81a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec81a-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ec81a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec81a-108">Retorne todos os grupos e unidades administrativas que o grupo é um membro de.</span><span class="sxs-lookup"><span data-stu-id="ec81a-108">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="ec81a-109">A seleção é transitiva.</span><span class="sxs-lookup"><span data-stu-id="ec81a-109">The check is transitive.</span></span> <span data-ttu-id="ec81a-110">Observação: Grupos não podem ser membros das funções de diretório, portanto nenhuma função de diretório será retornada.</span><span class="sxs-lookup"><span data-stu-id="ec81a-110">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec81a-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="ec81a-111">Permissions</span></span>
<span data-ttu-id="ec81a-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec81a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec81a-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec81a-114">Permission type</span></span>      | <span data-ttu-id="ec81a-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec81a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec81a-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec81a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ec81a-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec81a-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ec81a-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec81a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec81a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec81a-119">Not supported.</span></span>    |
|<span data-ttu-id="ec81a-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec81a-120">Application</span></span> | <span data-ttu-id="ec81a-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec81a-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec81a-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec81a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="ec81a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec81a-123">Request headers</span></span>
| <span data-ttu-id="ec81a-124">Nome</span><span class="sxs-lookup"><span data-stu-id="ec81a-124">Name</span></span>       | <span data-ttu-id="ec81a-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec81a-125">Type</span></span> | <span data-ttu-id="ec81a-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec81a-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ec81a-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec81a-127">Authorization</span></span>  | <span data-ttu-id="ec81a-128">string</span><span class="sxs-lookup"><span data-stu-id="ec81a-128">string</span></span>  | <span data-ttu-id="ec81a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec81a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec81a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec81a-131">Request body</span></span>
<span data-ttu-id="ec81a-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec81a-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ec81a-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ec81a-133">Parameter</span></span>    | <span data-ttu-id="ec81a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec81a-134">Type</span></span>   |<span data-ttu-id="ec81a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec81a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec81a-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ec81a-136">securityEnabledOnly</span></span>|<span data-ttu-id="ec81a-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec81a-137">Boolean</span></span>|<span data-ttu-id="ec81a-p106">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="ec81a-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="ec81a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec81a-140">Response</span></span>
<span data-ttu-id="ec81a-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="ec81a-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="ec81a-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec81a-142">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ec81a-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec81a-143">Request</span></span>
<span data-ttu-id="ec81a-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec81a-144">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="ec81a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec81a-145">Response</span></span>
<span data-ttu-id="ec81a-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec81a-146">The following is an example of the response.</span></span>
><span data-ttu-id="ec81a-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec81a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
