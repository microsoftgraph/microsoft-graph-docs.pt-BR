---
title: 'grupo: getMemberGroups'
description: Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação memberOf, que retorna somente os grupos dos quais o grupo é membro direto.
ms.openlocfilehash: a6778b37ef89444a47babbea8f11050e5ffcb974
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005033"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="2868d-104">grupo: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="2868d-104">group: getMemberGroups</span></span>

<span data-ttu-id="2868d-p102">Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [memberOf](../api/group-list-memberof.md), que retorna somente os grupos dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="2868d-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="2868d-p103">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="2868d-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="2868d-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="2868d-111">Permissions</span></span>

<span data-ttu-id="2868d-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2868d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2868d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2868d-114">Permission type</span></span>                        | <span data-ttu-id="2868d-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2868d-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="2868d-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2868d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="2868d-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2868d-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="2868d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2868d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2868d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2868d-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="2868d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2868d-120">Application</span></span>                            | <span data-ttu-id="2868d-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2868d-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="2868d-122">**Observação:** Essa API atualmente requer o `Directory.Read.All` permissão ou superior.</span><span class="sxs-lookup"><span data-stu-id="2868d-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="2868d-123">Usando o `Group.Read.All` permissão retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="2868d-123">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="2868d-124">Este é um bug conhecido.</span><span class="sxs-lookup"><span data-stu-id="2868d-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="2868d-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2868d-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="2868d-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2868d-126">Request headers</span></span>

| <span data-ttu-id="2868d-127">Nome</span><span class="sxs-lookup"><span data-stu-id="2868d-127">Name</span></span>          | <span data-ttu-id="2868d-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="2868d-128">Type</span></span>   | <span data-ttu-id="2868d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2868d-129">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="2868d-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="2868d-130">Authorization</span></span> | <span data-ttu-id="2868d-131">string</span><span class="sxs-lookup"><span data-stu-id="2868d-131">string</span></span> | <span data-ttu-id="2868d-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2868d-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2868d-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2868d-134">Request body</span></span>

<span data-ttu-id="2868d-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2868d-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2868d-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2868d-136">Parameter</span></span>           | <span data-ttu-id="2868d-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="2868d-137">Type</span></span>    | <span data-ttu-id="2868d-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="2868d-138">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="2868d-139">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="2868d-139">securityEnabledOnly</span></span> | <span data-ttu-id="2868d-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="2868d-140">Boolean</span></span> | <span data-ttu-id="2868d-p107">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="2868d-p107">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="2868d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2868d-143">Response</span></span>

<span data-ttu-id="2868d-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="2868d-144">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="2868d-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2868d-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2868d-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2868d-146">Request</span></span>

<span data-ttu-id="2868d-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2868d-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="2868d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="2868d-148">Response</span></span>

<span data-ttu-id="2868d-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2868d-149">The following is an example of the response.</span></span>

> <span data-ttu-id="2868d-150">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2868d-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2868d-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2868d-151">All the properties will be returned from an actual call.</span></span>

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
