---
title: 'usuário: getMemberGroups'
description: Retorne todos os grupos dos quais o usuário é membro. A verificação foi transitiva, ao contrário de leitura a
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a5f02e871dbda06df96caf7c9e66e7099673e034
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509161"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="6cd5e-104">usuário: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="6cd5e-104">user: getMemberGroups</span></span>

<span data-ttu-id="6cd5e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cd5e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6cd5e-p102">Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [member](../api/user-list-memberof.md), que retorna somente os grupos dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="6cd5e-p102">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="6cd5e-p103">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="6cd5e-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cd5e-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="6cd5e-112">Permissions</span></span>

<span data-ttu-id="6cd5e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cd5e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cd5e-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cd5e-115">Permission type</span></span>                        | <span data-ttu-id="6cd5e-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6cd5e-116">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6cd5e-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cd5e-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cd5e-118">User.ReadBasic.All and GroupMember.Read.All, User.Read and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read and Group.Read.All,  User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6cd5e-118">User.ReadBasic.All and GroupMember.Read.All, User.Read and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read and Group.Read.All,  User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="6cd5e-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cd5e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cd5e-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cd5e-120">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="6cd5e-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cd5e-121">Application</span></span>                            |  <span data-ttu-id="6cd5e-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd5e-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cd5e-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cd5e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="6cd5e-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cd5e-124">Request headers</span></span>

| <span data-ttu-id="6cd5e-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cd5e-125">Header</span></span>        | <span data-ttu-id="6cd5e-126">Valor</span><span class="sxs-lookup"><span data-stu-id="6cd5e-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="6cd5e-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cd5e-127">Authorization</span></span> | <span data-ttu-id="6cd5e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cd5e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6cd5e-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6cd5e-130">Content-Type</span></span>  | <span data-ttu-id="6cd5e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="6cd5e-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="6cd5e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cd5e-132">Request body</span></span>

<span data-ttu-id="6cd5e-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cd5e-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6cd5e-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6cd5e-134">Parameter</span></span>           | <span data-ttu-id="6cd5e-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cd5e-135">Type</span></span>    | <span data-ttu-id="6cd5e-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cd5e-136">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6cd5e-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="6cd5e-137">securityEnabledOnly</span></span> | <span data-ttu-id="6cd5e-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cd5e-138">Boolean</span></span> | <span data-ttu-id="6cd5e-p106">**true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário.</span><span class="sxs-lookup"><span data-stu-id="6cd5e-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="6cd5e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cd5e-141">Response</span></span>

<span data-ttu-id="6cd5e-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="6cd5e-142">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="6cd5e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cd5e-143">Example</span></span>

<span data-ttu-id="6cd5e-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6cd5e-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6cd5e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cd5e-145">Request</span></span>

<span data-ttu-id="6cd5e-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cd5e-146">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6cd5e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cd5e-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="6cd5e-148">C#</span><span class="sxs-lookup"><span data-stu-id="6cd5e-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cd5e-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cd5e-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cd5e-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cd5e-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cd5e-151">Java</span><span class="sxs-lookup"><span data-stu-id="6cd5e-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6cd5e-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cd5e-152">Response</span></span>

<span data-ttu-id="6cd5e-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cd5e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
