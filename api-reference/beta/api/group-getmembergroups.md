---
title: 'grupo: getMemberGroups'
description: Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação memberOf, que retorna somente os grupos dos quais o grupo é membro direto.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e485c80a06fc2d124dec728ab3ffcdfb8dcce105
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921532"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="66e68-104">grupo: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="66e68-104">group: getMemberGroups</span></span>

> <span data-ttu-id="66e68-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="66e68-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66e68-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="66e68-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66e68-p103">Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [memberOf](../api/group-list-memberof.md), que retorna somente os grupos dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="66e68-p103">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="66e68-p104">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="66e68-p104">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="66e68-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="66e68-113">Permissions</span></span>

<span data-ttu-id="66e68-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66e68-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66e68-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66e68-116">Permission type</span></span>                        | <span data-ttu-id="66e68-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66e68-117">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="66e68-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66e68-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="66e68-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66e68-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="66e68-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66e68-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66e68-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66e68-121">Not supported.</span></span>                                                                              |
| <span data-ttu-id="66e68-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66e68-122">Application</span></span>                            | <span data-ttu-id="66e68-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66e68-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="66e68-124">**Observação:** Essa API atualmente requer o `Directory.Read.All` permissão ou superior.</span><span class="sxs-lookup"><span data-stu-id="66e68-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="66e68-125">Usando o `Group.Read.All` permissão retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="66e68-125">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="66e68-126">Este é um bug conhecido.</span><span class="sxs-lookup"><span data-stu-id="66e68-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="66e68-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66e68-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="66e68-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66e68-128">Request headers</span></span>

| <span data-ttu-id="66e68-129">Nome</span><span class="sxs-lookup"><span data-stu-id="66e68-129">Name</span></span>          | <span data-ttu-id="66e68-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="66e68-130">Type</span></span>   | <span data-ttu-id="66e68-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="66e68-131">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="66e68-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="66e68-132">Authorization</span></span> | <span data-ttu-id="66e68-133">string</span><span class="sxs-lookup"><span data-stu-id="66e68-133">string</span></span> | <span data-ttu-id="66e68-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66e68-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66e68-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66e68-136">Request body</span></span>

<span data-ttu-id="66e68-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66e68-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="66e68-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="66e68-138">Parameter</span></span>           | <span data-ttu-id="66e68-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="66e68-139">Type</span></span>    | <span data-ttu-id="66e68-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="66e68-140">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="66e68-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="66e68-141">securityEnabledOnly</span></span> | <span data-ttu-id="66e68-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="66e68-142">Boolean</span></span> | <span data-ttu-id="66e68-p108">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="66e68-p108">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="66e68-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="66e68-145">Response</span></span>

<span data-ttu-id="66e68-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="66e68-146">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="66e68-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66e68-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="66e68-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66e68-148">Request</span></span>

<span data-ttu-id="66e68-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="66e68-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="66e68-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="66e68-150">Response</span></span>

<span data-ttu-id="66e68-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66e68-151">The following is an example of the response.</span></span>

> <span data-ttu-id="66e68-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66e68-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
