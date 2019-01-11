---
title: 'group: checkMemberGroups'
description: Verifique se a associação na lista especificada dos grupos. Retorna da lista os grupos dos quais
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 812377d3fe8677d877ac8faddce75c25732ff471
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861863"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="75817-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="75817-104">group: checkMemberGroups</span></span>

<span data-ttu-id="75817-p102">Verifique se há associação na lista de grupos especificada. Retorna os grupos da lista com os quais o grupo especificado tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="75817-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="75817-p103">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="75817-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="75817-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="75817-111">Permissions</span></span>

<span data-ttu-id="75817-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75817-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75817-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75817-114">Permission type</span></span>                        | <span data-ttu-id="75817-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75817-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="75817-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75817-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="75817-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="75817-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="75817-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75817-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75817-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75817-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="75817-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75817-120">Application</span></span>                            | <span data-ttu-id="75817-121">_Group.Read.All_, Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="75817-121">_Group.Read.All_, Directory.Read.All.</span></span> <span data-ttu-id="75817-122">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75817-122">Directory.ReadWrite.All</span></span>                               |

> <span data-ttu-id="75817-123">**Observação:** Essa API atualmente requer o `Directory.Read.All` permissão ou superior.</span><span class="sxs-lookup"><span data-stu-id="75817-123">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="75817-124">Usando o `Group.Read.All` permissão retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="75817-124">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="75817-125">Este é um bug conhecido.</span><span class="sxs-lookup"><span data-stu-id="75817-125">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="75817-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75817-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="75817-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75817-127">Request headers</span></span>

| <span data-ttu-id="75817-128">Nome</span><span class="sxs-lookup"><span data-stu-id="75817-128">Name</span></span>          | <span data-ttu-id="75817-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="75817-129">Type</span></span>   | <span data-ttu-id="75817-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="75817-130">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="75817-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="75817-131">Authorization</span></span> | <span data-ttu-id="75817-132">string</span><span class="sxs-lookup"><span data-stu-id="75817-132">string</span></span> | <span data-ttu-id="75817-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75817-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75817-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75817-135">Request body</span></span>

<span data-ttu-id="75817-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75817-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="75817-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="75817-137">Parameter</span></span> | <span data-ttu-id="75817-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="75817-138">Type</span></span>              | <span data-ttu-id="75817-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="75817-139">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="75817-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="75817-140">groupIds</span></span>  | <span data-ttu-id="75817-141">String collection</span><span class="sxs-lookup"><span data-stu-id="75817-141">String collection</span></span> | <span data-ttu-id="75817-142">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="75817-142">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="75817-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="75817-143">Response</span></span>

<span data-ttu-id="75817-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75817-144">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75817-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75817-145">Example</span></span>

<span data-ttu-id="75817-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="75817-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="75817-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75817-147">Request</span></span>

<span data-ttu-id="75817-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75817-148">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="75817-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="75817-149">Response</span></span>

<span data-ttu-id="75817-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75817-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
