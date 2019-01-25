---
title: Obter grupos de membros
description: Retornar todos os grupos que o usuário especificado, o grupo, o serviço principal ou o objeto de diretório é um membro de. Essa função é transitiva.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9ab73b691ed9cfa4c756e4f0134adf9df7350aae
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526169"
---
# <a name="get-member-groups"></a><span data-ttu-id="9c1c2-104">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="9c1c2-104">Get member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c1c2-105">Retornar todos os grupos que o usuário especificado, o grupo, o serviço principal ou o objeto de diretório é um membro de.</span><span class="sxs-lookup"><span data-stu-id="9c1c2-105">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="9c1c2-106">Essa função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="9c1c2-106">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c1c2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c1c2-107">Permissions</span></span>
<span data-ttu-id="9c1c2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c1c2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9c1c2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c1c2-110">Permission type</span></span>      | <span data-ttu-id="9c1c2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c1c2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c1c2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c1c2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c1c2-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c1c2-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="9c1c2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c1c2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c1c2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c1c2-115">Not supported.</span></span>    |
|<span data-ttu-id="9c1c2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c1c2-116">Application</span></span> | <span data-ttu-id="9c1c2-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c1c2-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c1c2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c1c2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="9c1c2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1c2-119">Request headers</span></span>
| <span data-ttu-id="9c1c2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9c1c2-120">Name</span></span>       | <span data-ttu-id="9c1c2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c1c2-121">Type</span></span> | <span data-ttu-id="9c1c2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c1c2-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c1c2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c1c2-123">Authorization</span></span>  | <span data-ttu-id="9c1c2-124">string</span><span class="sxs-lookup"><span data-stu-id="9c1c2-124">string</span></span>  | <span data-ttu-id="9c1c2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c1c2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c1c2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c1c2-127">Content-Type</span></span>  | <span data-ttu-id="9c1c2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9c1c2-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c1c2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1c2-129">Request body</span></span>
<span data-ttu-id="9c1c2-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c1c2-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9c1c2-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9c1c2-131">Parameter</span></span>    | <span data-ttu-id="9c1c2-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c1c2-132">Type</span></span>   |<span data-ttu-id="9c1c2-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c1c2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c1c2-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="9c1c2-134">securityEnabledOnly</span></span>|<span data-ttu-id="9c1c2-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="9c1c2-135">Boolean</span></span>| <span data-ttu-id="9c1c2-p105">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="9c1c2-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="9c1c2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c1c2-138">Response</span></span>

<span data-ttu-id="9c1c2-139">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c1c2-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c1c2-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c1c2-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9c1c2-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1c2-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="9c1c2-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c1c2-142">Response</span></span>
<span data-ttu-id="9c1c2-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c1c2-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-getmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
