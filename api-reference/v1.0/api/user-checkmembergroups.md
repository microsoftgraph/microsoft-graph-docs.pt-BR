---
title: checkMemberGroups
description: Verifique se há associação na lista de grupos especificada. Retorna da lista aqueles grupos dos quais
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 272b377534bd9fbee676135240d85983bf0f121b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460557"
---
# <a name="checkmembergroups"></a><span data-ttu-id="9ab8f-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="9ab8f-104">checkMemberGroups</span></span>

<span data-ttu-id="9ab8f-p102">Verifique se há associação na lista de grupos especificada. Retorna da lista os grupos com os quais o usuário tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="9ab8f-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="9ab8f-p103">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="9ab8f-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ab8f-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ab8f-111">Permissions</span></span>

<span data-ttu-id="9ab8f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ab8f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ab8f-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ab8f-114">Permission type</span></span>                        | <span data-ttu-id="9ab8f-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ab8f-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9ab8f-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ab8f-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ab8f-117">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ab8f-117">User.Read and Group.Read.All, User.ReadBasic.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="9ab8f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ab8f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ab8f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ab8f-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="9ab8f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ab8f-120">Application</span></span>                            | <span data-ttu-id="9ab8f-121">User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ab8f-121">User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ab8f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab8f-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="9ab8f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab8f-123">Request headers</span></span>

| <span data-ttu-id="9ab8f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ab8f-124">Header</span></span>        | <span data-ttu-id="9ab8f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="9ab8f-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="9ab8f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ab8f-126">Authorization</span></span> | <span data-ttu-id="9ab8f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ab8f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ab8f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ab8f-129">Content-Type</span></span>  | <span data-ttu-id="9ab8f-130">application/json</span><span class="sxs-lookup"><span data-stu-id="9ab8f-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="9ab8f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab8f-131">Request body</span></span>

<span data-ttu-id="9ab8f-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ab8f-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9ab8f-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9ab8f-133">Parameter</span></span> | <span data-ttu-id="9ab8f-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ab8f-134">Type</span></span>              | <span data-ttu-id="9ab8f-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ab8f-135">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="9ab8f-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="9ab8f-136">groupIds</span></span>  | <span data-ttu-id="9ab8f-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ab8f-137">String collection</span></span> | <span data-ttu-id="9ab8f-138">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="9ab8f-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="9ab8f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab8f-139">Response</span></span>

<span data-ttu-id="9ab8f-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ab8f-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ab8f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ab8f-141">Example</span></span>

<span data-ttu-id="9ab8f-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9ab8f-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9ab8f-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab8f-143">Request</span></span>

<span data-ttu-id="9ab8f-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ab8f-144">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9ab8f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab8f-145">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ab8f-146">C#</span><span class="sxs-lookup"><span data-stu-id="9ab8f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ab8f-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="9ab8f-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ab8f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ab8f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9ab8f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab8f-149">Response</span></span>

<span data-ttu-id="9ab8f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ab8f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
