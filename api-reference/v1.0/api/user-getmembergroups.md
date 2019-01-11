---
title: 'usuário: getMemberGroups'
description: Retorne todos os grupos que o usuário é membro de. A seleção é transitiva, ao contrário de leitura a
localization_priority: Priority
ms.openlocfilehash: 23b05799d6660b2b173f7e5dbd1c8d86f0644fef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870060"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="911de-104">usuário: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="911de-104">user: getMemberGroups</span></span>

<span data-ttu-id="911de-p102">Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [member](../api/user-list-memberof.md), que retorna somente os grupos dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="911de-p102">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="911de-p103">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="911de-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="911de-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="911de-111">Permissions</span></span>

<span data-ttu-id="911de-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="911de-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="911de-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="911de-114">Permission type</span></span>                        | <span data-ttu-id="911de-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="911de-115">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="911de-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="911de-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="911de-117">~~User.Read and Group.Read.All~~, ~~User.ReadBasic.All and Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="911de-117">~~User.Read and Group.Read.All~~, ~~User.ReadBasic.All and Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="911de-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="911de-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="911de-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="911de-119">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="911de-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="911de-120">Application</span></span>                            | <span data-ttu-id="911de-121">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="911de-121">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span></span>                                                                                        |

> <span data-ttu-id="911de-122">**Observação:** Essa API atualmente requer o `Directory.Read.All` permissão ou superior.</span><span class="sxs-lookup"><span data-stu-id="911de-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="911de-123">Usando a permissão Group.Read.All, sozinhos ou em combinação com um `User.` permissão, retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="911de-123">Using the Group.Read.All permission, either alone or in combination with a `User.` permission, will return an error.</span></span> <span data-ttu-id="911de-124">Este é um bug conhecido.</span><span class="sxs-lookup"><span data-stu-id="911de-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="911de-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="911de-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="911de-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="911de-126">Request headers</span></span>

| <span data-ttu-id="911de-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="911de-127">Header</span></span>        | <span data-ttu-id="911de-128">Valor</span><span class="sxs-lookup"><span data-stu-id="911de-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="911de-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="911de-129">Authorization</span></span> | <span data-ttu-id="911de-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="911de-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="911de-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="911de-132">Content-Type</span></span>  | <span data-ttu-id="911de-133">application/json</span><span class="sxs-lookup"><span data-stu-id="911de-133">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="911de-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="911de-134">Request body</span></span>

<span data-ttu-id="911de-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="911de-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="911de-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="911de-136">Parameter</span></span>           | <span data-ttu-id="911de-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="911de-137">Type</span></span>    | <span data-ttu-id="911de-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="911de-138">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="911de-139">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="911de-139">securityEnabledOnly</span></span> | <span data-ttu-id="911de-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="911de-140">Boolean</span></span> | <span data-ttu-id="911de-p107">**true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário.</span><span class="sxs-lookup"><span data-stu-id="911de-p107">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="911de-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="911de-143">Response</span></span>

<span data-ttu-id="911de-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="911de-144">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="911de-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="911de-145">Example</span></span>

<span data-ttu-id="911de-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="911de-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="911de-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="911de-147">Request</span></span>

<span data-ttu-id="911de-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="911de-148">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="911de-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="911de-149">Response</span></span>

<span data-ttu-id="911de-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="911de-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
