---
title: checkMemberGroups
description: Verifique se a associação na lista especificada dos grupos. Retorna da lista os grupos dos quais
author: dkershaw10
ms.openlocfilehash: 613faacdbd2651700f264cdf89ec396b54752b76
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310595"
---
# <a name="checkmembergroups"></a><span data-ttu-id="8c489-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="8c489-104">checkMemberGroups</span></span>

> <span data-ttu-id="8c489-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8c489-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c489-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8c489-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8c489-p103">Verifique se há associação na lista de grupos especificada. Retorna da lista os grupos com os quais o usuário tem uma associação direta ou transitiva.</span><span class="sxs-lookup"><span data-stu-id="8c489-p103">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="8c489-p104">Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="8c489-p104">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c489-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c489-113">Permissions</span></span>

<span data-ttu-id="8c489-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c489-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c489-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c489-116">Permission type</span></span>                        | <span data-ttu-id="8c489-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c489-117">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8c489-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c489-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c489-119">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c489-119">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="8c489-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c489-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c489-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c489-121">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="8c489-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c489-122">Application</span></span>                            | <span data-ttu-id="8c489-123">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c489-123">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="8c489-124">**Observação:** Essa API atualmente requer o `Directory.Read.All` permissão ou superior.</span><span class="sxs-lookup"><span data-stu-id="8c489-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="8c489-125">Usando o `User.Read.All` ou `User.ReadWrite.All` permissões retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="8c489-125">Using the `User.Read.All` or `User.ReadWrite.All` permissions will return an error.</span></span> <span data-ttu-id="8c489-126">Este é um bug conhecido.</span><span class="sxs-lookup"><span data-stu-id="8c489-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="8c489-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c489-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="8c489-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c489-128">Request headers</span></span>

| <span data-ttu-id="8c489-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c489-129">Header</span></span>        | <span data-ttu-id="8c489-130">Valor</span><span class="sxs-lookup"><span data-stu-id="8c489-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="8c489-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c489-131">Authorization</span></span> | <span data-ttu-id="8c489-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c489-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c489-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c489-134">Content-Type</span></span>  | <span data-ttu-id="8c489-135">application/json</span><span class="sxs-lookup"><span data-stu-id="8c489-135">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="8c489-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c489-136">Request body</span></span>

<span data-ttu-id="8c489-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c489-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c489-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8c489-138">Parameter</span></span> | <span data-ttu-id="8c489-139">Type</span><span class="sxs-lookup"><span data-stu-id="8c489-139">Type</span></span>   | <span data-ttu-id="8c489-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c489-140">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="8c489-141">groupIds</span><span class="sxs-lookup"><span data-stu-id="8c489-141">groupIds</span></span>  | <span data-ttu-id="8c489-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c489-142">String</span></span> | <span data-ttu-id="8c489-143">Uma matriz de IDs de grupo</span><span class="sxs-lookup"><span data-stu-id="8c489-143">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="8c489-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c489-144">Response</span></span>

<span data-ttu-id="8c489-145">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c489-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c489-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c489-146">Example</span></span>

<span data-ttu-id="8c489-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8c489-147">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8c489-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c489-148">Request</span></span>

<span data-ttu-id="8c489-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c489-149">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="8c489-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c489-150">Response</span></span>

<span data-ttu-id="8c489-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c489-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
