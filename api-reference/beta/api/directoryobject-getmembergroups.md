---
title: Obter grupos de membros
description: Retornar todos os grupos que o usuário especificado, o grupo, o serviço principal ou o objeto de diretório é um membro de. Essa função é transitiva.
localization_priority: Normal
ms.openlocfilehash: 1e9cc785bccd9b5bc6d1c7e3da8d38874a440cf3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808796"
---
# <a name="get-member-groups"></a><span data-ttu-id="3ed05-104">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="3ed05-104">Get member groups</span></span>

> <span data-ttu-id="3ed05-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3ed05-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ed05-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3ed05-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ed05-107">Retornar todos os grupos que o usuário especificado, o grupo, o serviço principal ou o objeto de diretório é um membro de.</span><span class="sxs-lookup"><span data-stu-id="3ed05-107">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="3ed05-108">Essa função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="3ed05-108">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ed05-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="3ed05-109">Permissions</span></span>
<span data-ttu-id="3ed05-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ed05-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3ed05-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ed05-112">Permission type</span></span>      | <span data-ttu-id="3ed05-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ed05-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ed05-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ed05-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3ed05-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ed05-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="3ed05-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ed05-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ed05-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ed05-117">Not supported.</span></span>    |
|<span data-ttu-id="3ed05-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ed05-118">Application</span></span> | <span data-ttu-id="3ed05-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ed05-119">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ed05-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ed05-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="3ed05-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ed05-121">Request headers</span></span>
| <span data-ttu-id="3ed05-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3ed05-122">Name</span></span>       | <span data-ttu-id="3ed05-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ed05-123">Type</span></span> | <span data-ttu-id="3ed05-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ed05-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ed05-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ed05-125">Authorization</span></span>  | <span data-ttu-id="3ed05-126">string</span><span class="sxs-lookup"><span data-stu-id="3ed05-126">string</span></span>  | <span data-ttu-id="3ed05-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ed05-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ed05-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ed05-129">Content-Type</span></span>  | <span data-ttu-id="3ed05-130">application/json</span><span class="sxs-lookup"><span data-stu-id="3ed05-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ed05-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ed05-131">Request body</span></span>
<span data-ttu-id="3ed05-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ed05-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3ed05-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3ed05-133">Parameter</span></span>    | <span data-ttu-id="3ed05-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ed05-134">Type</span></span>   |<span data-ttu-id="3ed05-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ed05-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ed05-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="3ed05-136">securityEnabledOnly</span></span>|<span data-ttu-id="3ed05-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="3ed05-137">Boolean</span></span>| <span data-ttu-id="3ed05-p106">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="3ed05-p106">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="3ed05-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ed05-140">Response</span></span>

<span data-ttu-id="3ed05-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ed05-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ed05-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ed05-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3ed05-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ed05-143">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="3ed05-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ed05-144">Response</span></span>
<span data-ttu-id="3ed05-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ed05-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
