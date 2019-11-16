---
title: 'usuário: getMemberGroups'
description: Retorne todos os grupos dos quais o usuário é membro. A verificação foi transitiva, ao contrário de leitura a
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1972411aac620b982012c6127739adb4e20e784d
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658888"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="7dec5-104">usuário: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="7dec5-104">user: getMemberGroups</span></span>

<span data-ttu-id="7dec5-p102">Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [member](../api/user-list-memberof.md), que retorna somente os grupos dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="7dec5-p102">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="7dec5-p103">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="7dec5-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dec5-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="7dec5-111">Permissions</span></span>

<span data-ttu-id="7dec5-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dec5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7dec5-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dec5-114">Permission type</span></span>                        | <span data-ttu-id="7dec5-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7dec5-115">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7dec5-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dec5-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="7dec5-117">User.ReadBasic.All and GroupMember.Read.All, User.Read and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read and Group.Read.All,  User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7dec5-117">User.ReadBasic.All and GroupMember.Read.All, User.Read and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read and Group.Read.All,  User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="7dec5-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dec5-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dec5-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dec5-119">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="7dec5-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dec5-120">Application</span></span>                            |  <span data-ttu-id="7dec5-121">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dec5-121">User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dec5-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dec5-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="7dec5-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dec5-123">Request headers</span></span>

| <span data-ttu-id="7dec5-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7dec5-124">Header</span></span>        | <span data-ttu-id="7dec5-125">Valor</span><span class="sxs-lookup"><span data-stu-id="7dec5-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="7dec5-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dec5-126">Authorization</span></span> | <span data-ttu-id="7dec5-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dec5-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7dec5-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7dec5-129">Content-Type</span></span>  | <span data-ttu-id="7dec5-130">application/json</span><span class="sxs-lookup"><span data-stu-id="7dec5-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="7dec5-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dec5-131">Request body</span></span>

<span data-ttu-id="7dec5-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dec5-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7dec5-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7dec5-133">Parameter</span></span>           | <span data-ttu-id="7dec5-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dec5-134">Type</span></span>    | <span data-ttu-id="7dec5-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dec5-135">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7dec5-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="7dec5-136">securityEnabledOnly</span></span> | <span data-ttu-id="7dec5-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="7dec5-137">Boolean</span></span> | <span data-ttu-id="7dec5-p106">**true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário.</span><span class="sxs-lookup"><span data-stu-id="7dec5-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="7dec5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dec5-140">Response</span></span>

<span data-ttu-id="7dec5-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="7dec5-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="7dec5-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dec5-142">Example</span></span>

<span data-ttu-id="7dec5-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7dec5-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7dec5-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dec5-144">Request</span></span>

<span data-ttu-id="7dec5-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dec5-145">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7dec5-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dec5-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7dec5-147">C#</span><span class="sxs-lookup"><span data-stu-id="7dec5-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7dec5-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dec5-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7dec5-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dec5-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7dec5-150">Java</span><span class="sxs-lookup"><span data-stu-id="7dec5-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7dec5-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dec5-151">Response</span></span>

<span data-ttu-id="7dec5-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7dec5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
