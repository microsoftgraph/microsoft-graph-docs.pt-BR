---
title: Verificar grupos de membros
description: Verificar a associação em uma lista especificada de grupos e retorna a partir dessa lista desses grupos
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 53c89a6dd6fb0c16e0df7c6035ed0667c227787d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522522"
---
# <a name="check-member-groups"></a><span data-ttu-id="a6ecf-103">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="a6ecf-103">Check member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6ecf-104">Verifique se a associação em uma lista especificada de grupos e retorna a partir dessa lista esses grupos dos quais o usuário especificado, o grupo, o serviço principal ou o objeto de diretório é membro.</span><span class="sxs-lookup"><span data-stu-id="a6ecf-104">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="a6ecf-105">Essa função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a6ecf-105">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6ecf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6ecf-106">Permissions</span></span>
<span data-ttu-id="a6ecf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6ecf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a6ecf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6ecf-109">Permission type</span></span>      | <span data-ttu-id="a6ecf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6ecf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6ecf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6ecf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a6ecf-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6ecf-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="a6ecf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6ecf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6ecf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6ecf-114">Not supported.</span></span>    |
|<span data-ttu-id="a6ecf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6ecf-115">Application</span></span> | <span data-ttu-id="a6ecf-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6ecf-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6ecf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6ecf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servciePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="a6ecf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ecf-118">Request headers</span></span>
| <span data-ttu-id="a6ecf-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a6ecf-119">Name</span></span>       | <span data-ttu-id="a6ecf-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6ecf-120">Type</span></span> | <span data-ttu-id="a6ecf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6ecf-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a6ecf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6ecf-122">Authorization</span></span>  | <span data-ttu-id="a6ecf-123">string</span><span class="sxs-lookup"><span data-stu-id="a6ecf-123">string</span></span>  | <span data-ttu-id="a6ecf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6ecf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a6ecf-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6ecf-126">Content-Type</span></span>  | <span data-ttu-id="a6ecf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a6ecf-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6ecf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ecf-128">Request body</span></span>
<span data-ttu-id="a6ecf-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6ecf-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a6ecf-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a6ecf-130">Parameter</span></span>    | <span data-ttu-id="a6ecf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6ecf-131">Type</span></span>   |<span data-ttu-id="a6ecf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6ecf-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6ecf-133">groupIds</span><span class="sxs-lookup"><span data-stu-id="a6ecf-133">groupIds</span></span>|<span data-ttu-id="a6ecf-134">String</span><span class="sxs-lookup"><span data-stu-id="a6ecf-134">String</span></span>|<span data-ttu-id="a6ecf-p104">Uma coleção que contém as IDs de objetos dos grupos em que se deve verificar a associação. Até 20 grupos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="a6ecf-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="a6ecf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6ecf-137">Response</span></span>

<span data-ttu-id="a6ecf-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6ecf-138">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6ecf-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6ecf-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a6ecf-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ecf-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="a6ecf-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6ecf-141">Response</span></span>
<span data-ttu-id="a6ecf-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6ecf-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
