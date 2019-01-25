---
title: 'user: getMemberObjects'
description: Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 219e996bdf9b796cdd6a000b988e0f2ac73023ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509984"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="fa90c-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="fa90c-104">user: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa90c-p102">Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="fa90c-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa90c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa90c-107">Permissions</span></span>
<span data-ttu-id="fa90c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa90c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fa90c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa90c-110">Permission type</span></span>      | <span data-ttu-id="fa90c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa90c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa90c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa90c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fa90c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa90c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa90c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa90c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa90c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa90c-115">Not supported.</span></span>    |
|<span data-ttu-id="fa90c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa90c-116">Application</span></span> | <span data-ttu-id="fa90c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa90c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa90c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa90c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="fa90c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa90c-119">Request headers</span></span>
| <span data-ttu-id="fa90c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa90c-120">Header</span></span>       | <span data-ttu-id="fa90c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fa90c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa90c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa90c-122">Authorization</span></span>  | <span data-ttu-id="fa90c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa90c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fa90c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa90c-125">Content-Type</span></span>  | <span data-ttu-id="fa90c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa90c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa90c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa90c-127">Request body</span></span>
<span data-ttu-id="fa90c-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa90c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa90c-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fa90c-129">Parameter</span></span>    | <span data-ttu-id="fa90c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa90c-130">Type</span></span>   |<span data-ttu-id="fa90c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa90c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa90c-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="fa90c-132">securityEnabledOnly</span></span>|<span data-ttu-id="fa90c-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="fa90c-133">Boolean</span></span>|<span data-ttu-id="fa90c-p105">**true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário.</span><span class="sxs-lookup"><span data-stu-id="fa90c-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="fa90c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa90c-136">Response</span></span>

<span data-ttu-id="fa90c-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos e das funções de diretório dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="fa90c-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="fa90c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa90c-138">Example</span></span>
<span data-ttu-id="fa90c-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fa90c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fa90c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa90c-140">Request</span></span>
<span data-ttu-id="fa90c-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa90c-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="fa90c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa90c-142">Response</span></span>
<span data-ttu-id="fa90c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa90c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-getmemberobjects.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
