---
title: 'grupo: getMemberGroups'
description: Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação memberOf, que retorna somente os grupos dos quais o grupo é membro direto.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: a5a6472427960d6e6179a80114fe9c9205e9e022
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529240"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="d61a6-104">grupo: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="d61a6-104">group: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d61a6-p102">Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [memberOf](../api/group-list-memberof.md), que retorna somente os grupos dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="d61a6-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="d61a6-p103">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="d61a6-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="d61a6-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="d61a6-111">Permissions</span></span>

<span data-ttu-id="d61a6-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d61a6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d61a6-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d61a6-114">Permission type</span></span>                        | <span data-ttu-id="d61a6-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d61a6-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="d61a6-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d61a6-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d61a6-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d61a6-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="d61a6-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d61a6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d61a6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d61a6-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="d61a6-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d61a6-120">Application</span></span>                            | <span data-ttu-id="d61a6-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d61a6-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="d61a6-122">**Observação:** esta API atualmente exige o `Directory.Read.All` permissão ou posterior.</span><span class="sxs-lookup"><span data-stu-id="d61a6-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="d61a6-123">Usando o `Group.Read.All` permissão retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="d61a6-123">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="d61a6-124">Este é um bug conhecido.</span><span class="sxs-lookup"><span data-stu-id="d61a6-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="d61a6-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d61a6-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="d61a6-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d61a6-126">Request headers</span></span>

| <span data-ttu-id="d61a6-127">Nome</span><span class="sxs-lookup"><span data-stu-id="d61a6-127">Name</span></span>          | <span data-ttu-id="d61a6-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="d61a6-128">Type</span></span>   | <span data-ttu-id="d61a6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d61a6-129">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="d61a6-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="d61a6-130">Authorization</span></span> | <span data-ttu-id="d61a6-131">string</span><span class="sxs-lookup"><span data-stu-id="d61a6-131">string</span></span> | <span data-ttu-id="d61a6-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d61a6-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d61a6-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d61a6-134">Request body</span></span>

<span data-ttu-id="d61a6-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d61a6-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d61a6-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d61a6-136">Parameter</span></span>           | <span data-ttu-id="d61a6-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="d61a6-137">Type</span></span>    | <span data-ttu-id="d61a6-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="d61a6-138">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="d61a6-139">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="d61a6-139">securityEnabledOnly</span></span> | <span data-ttu-id="d61a6-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="d61a6-140">Boolean</span></span> | <span data-ttu-id="d61a6-p107">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="d61a6-p107">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="d61a6-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d61a6-143">Response</span></span>

<span data-ttu-id="d61a6-144">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="d61a6-144">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="d61a6-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d61a6-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d61a6-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d61a6-146">Request</span></span>

<span data-ttu-id="d61a6-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d61a6-147">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d61a6-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d61a6-148">Response</span></span>

<span data-ttu-id="d61a6-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d61a6-149">The following is an example of the response.</span></span>

> <span data-ttu-id="d61a6-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d61a6-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-getmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
