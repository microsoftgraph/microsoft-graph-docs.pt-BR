---
title: Verificar grupos de membros
description: Verificar a associação em uma lista especificada de grupos e retorna a partir dessa lista desses grupos
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93ff0a0cb215e489490e50bde40f56e5b562be95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971085"
---
# <a name="check-member-groups"></a><span data-ttu-id="5ff74-103">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="5ff74-103">Check member groups</span></span>

> <span data-ttu-id="5ff74-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5ff74-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ff74-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5ff74-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ff74-106">Verifique se a associação em uma lista especificada de grupos e retorna a partir dessa lista esses grupos dos quais o usuário especificado, o grupo, o serviço principal ou o objeto de diretório é membro.</span><span class="sxs-lookup"><span data-stu-id="5ff74-106">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="5ff74-107">Essa função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="5ff74-107">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ff74-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ff74-108">Permissions</span></span>
<span data-ttu-id="5ff74-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ff74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5ff74-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ff74-111">Permission type</span></span>      | <span data-ttu-id="5ff74-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ff74-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ff74-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ff74-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5ff74-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ff74-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="5ff74-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ff74-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ff74-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ff74-116">Not supported.</span></span>    |
|<span data-ttu-id="5ff74-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ff74-117">Application</span></span> | <span data-ttu-id="5ff74-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ff74-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ff74-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ff74-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servciePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="5ff74-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ff74-120">Request headers</span></span>
| <span data-ttu-id="5ff74-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5ff74-121">Name</span></span>       | <span data-ttu-id="5ff74-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ff74-122">Type</span></span> | <span data-ttu-id="5ff74-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ff74-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5ff74-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ff74-124">Authorization</span></span>  | <span data-ttu-id="5ff74-125">string</span><span class="sxs-lookup"><span data-stu-id="5ff74-125">string</span></span>  | <span data-ttu-id="5ff74-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ff74-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ff74-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ff74-128">Content-Type</span></span>  | <span data-ttu-id="5ff74-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5ff74-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ff74-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ff74-130">Request body</span></span>
<span data-ttu-id="5ff74-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ff74-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5ff74-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5ff74-132">Parameter</span></span>    | <span data-ttu-id="5ff74-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ff74-133">Type</span></span>   |<span data-ttu-id="5ff74-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ff74-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ff74-135">groupIds</span><span class="sxs-lookup"><span data-stu-id="5ff74-135">groupIds</span></span>|<span data-ttu-id="5ff74-136">String</span><span class="sxs-lookup"><span data-stu-id="5ff74-136">String</span></span>|<span data-ttu-id="5ff74-p105">Uma coleção que contém as IDs de objetos dos grupos em que se deve verificar a associação. Até 20 grupos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="5ff74-p105">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="5ff74-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ff74-139">Response</span></span>

<span data-ttu-id="5ff74-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ff74-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ff74-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ff74-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5ff74-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ff74-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="5ff74-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ff74-143">Response</span></span>
<span data-ttu-id="5ff74-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ff74-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
