---
title: 'group: checkMemberGroups'
description: Verifique se há associação na lista de grupos especificada. Retorna da lista aqueles grupos dos quais
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 1815f187a25eaddbd3b1757fde5e7e4e9c74f650
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329614"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="65562-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="65562-104">group: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65562-p102">Verifique se há associação na lista de grupos especificada. Retorna os grupos da lista com os quais o grupo especificado tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="65562-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="65562-p103">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="65562-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="65562-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="65562-111">Permissions</span></span>

<span data-ttu-id="65562-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65562-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65562-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65562-114">Permission type</span></span>                        | <span data-ttu-id="65562-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65562-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="65562-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65562-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="65562-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65562-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="65562-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65562-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65562-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65562-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="65562-120">Application</span><span class="sxs-lookup"><span data-stu-id="65562-120">Application</span></span>                            | <span data-ttu-id="65562-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65562-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="65562-122">**Observação:** esta API atualmente exige o `Directory.Read.All` permissão ou posterior.</span><span class="sxs-lookup"><span data-stu-id="65562-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="65562-123">Usando a permissão `Group.Read.All` retornarão um erro.</span><span class="sxs-lookup"><span data-stu-id="65562-123">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="65562-124">Este é um bug conhecido.</span><span class="sxs-lookup"><span data-stu-id="65562-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="65562-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65562-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="65562-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65562-126">Request headers</span></span>

| <span data-ttu-id="65562-127">Nome</span><span class="sxs-lookup"><span data-stu-id="65562-127">Name</span></span>          | <span data-ttu-id="65562-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="65562-128">Type</span></span>   | <span data-ttu-id="65562-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="65562-129">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="65562-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="65562-130">Authorization</span></span> | <span data-ttu-id="65562-131">string</span><span class="sxs-lookup"><span data-stu-id="65562-131">string</span></span> | <span data-ttu-id="65562-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65562-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65562-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65562-134">Request body</span></span>

<span data-ttu-id="65562-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65562-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="65562-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="65562-136">Parameter</span></span> | <span data-ttu-id="65562-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="65562-137">Type</span></span>   | <span data-ttu-id="65562-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="65562-138">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="65562-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="65562-139">groupIds</span></span>  | <span data-ttu-id="65562-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="65562-140">String collection</span></span> | <span data-ttu-id="65562-141">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="65562-141">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="65562-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="65562-142">Response</span></span>

<span data-ttu-id="65562-143">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65562-143">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65562-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65562-144">Example</span></span>

<span data-ttu-id="65562-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="65562-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="65562-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65562-146">Request</span></span>

<span data-ttu-id="65562-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65562-147">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="65562-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="65562-148">Response</span></span>

<span data-ttu-id="65562-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65562-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
