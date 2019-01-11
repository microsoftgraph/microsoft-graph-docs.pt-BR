---
title: Obter objetos de membros
description: " Retorna todos os grupos, unidades administrativas e funções de diretório que um usuário, grupo, entidades de serviço ou objeto de diretório é um membro de. Essa função é transitiva. "
localization_priority: Normal
ms.openlocfilehash: f63c077414f656df168db5c5af498cec0f79e703
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874799"
---
# <a name="get-member-objects"></a><span data-ttu-id="ec70d-104">Obter objetos de membros</span><span class="sxs-lookup"><span data-stu-id="ec70d-104">Get member objects</span></span>

> <span data-ttu-id="ec70d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ec70d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec70d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ec70d-106">Use of these APIs in production applications is not supported.</span></span>

 <span data-ttu-id="ec70d-107">Retorna todos os grupos, unidades administrativas e funções de diretório que um usuário, grupo, entidades de serviço ou objeto de diretório é um membro de.</span><span class="sxs-lookup"><span data-stu-id="ec70d-107">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="ec70d-108">Essa função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="ec70d-108">This function is transitive.</span></span> 
 > <span data-ttu-id="ec70d-109">Observação: Somente usuários podem ser membros de funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="ec70d-109">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec70d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec70d-110">Permissions</span></span>
<span data-ttu-id="ec70d-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec70d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ec70d-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec70d-113">Permission type</span></span>      | <span data-ttu-id="ec70d-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec70d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec70d-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec70d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ec70d-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec70d-116">Directory.Read.All</span></span>    |
|<span data-ttu-id="ec70d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec70d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec70d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec70d-118">Not supported.</span></span>    |
|<span data-ttu-id="ec70d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec70d-119">Application</span></span> | <span data-ttu-id="ec70d-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec70d-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec70d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec70d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="ec70d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec70d-122">Request headers</span></span>
| <span data-ttu-id="ec70d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ec70d-123">Name</span></span>       | <span data-ttu-id="ec70d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec70d-124">Type</span></span> | <span data-ttu-id="ec70d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec70d-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ec70d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec70d-126">Authorization</span></span>  | <span data-ttu-id="ec70d-127">string</span><span class="sxs-lookup"><span data-stu-id="ec70d-127">string</span></span>  | <span data-ttu-id="ec70d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec70d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec70d-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec70d-130">Content-Type</span></span>  | <span data-ttu-id="ec70d-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ec70d-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec70d-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec70d-132">Request body</span></span>
<span data-ttu-id="ec70d-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec70d-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ec70d-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ec70d-134">Parameter</span></span>    | <span data-ttu-id="ec70d-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec70d-135">Type</span></span>   |<span data-ttu-id="ec70d-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec70d-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec70d-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ec70d-137">securityEnabledOnly</span></span>|<span data-ttu-id="ec70d-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec70d-138">Boolean</span></span>| <span data-ttu-id="ec70d-p106">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="ec70d-p106">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="ec70d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec70d-141">Response</span></span>

<span data-ttu-id="ec70d-142">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec70d-142">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec70d-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec70d-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ec70d-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec70d-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="ec70d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec70d-145">Response</span></span>
<span data-ttu-id="ec70d-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec70d-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
