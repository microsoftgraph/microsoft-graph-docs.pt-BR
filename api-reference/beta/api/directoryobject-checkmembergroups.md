---
title: Verificar grupos de membros
description: Verificar se há associação em uma lista de grupos especificada e retorna dessa lista esses grupos
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 53c89a6dd6fb0c16e0df7c6035ed0667c227787d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455188"
---
# <a name="check-member-groups"></a><span data-ttu-id="0893d-103">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="0893d-103">Check member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0893d-104">Verifique se há associação em uma lista especificada de grupos e retorna dessa lista os grupos dos quais o usuário, grupo, entidade de serviço ou objeto de diretório especificado é um membro.</span><span class="sxs-lookup"><span data-stu-id="0893d-104">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="0893d-105">Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="0893d-105">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="0893d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0893d-106">Permissions</span></span>
<span data-ttu-id="0893d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0893d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0893d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0893d-109">Permission type</span></span>      | <span data-ttu-id="0893d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0893d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0893d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0893d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0893d-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0893d-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="0893d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0893d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0893d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0893d-114">Not supported.</span></span>    |
|<span data-ttu-id="0893d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0893d-115">Application</span></span> | <span data-ttu-id="0893d-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0893d-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0893d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0893d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servciePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="0893d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0893d-118">Request headers</span></span>
| <span data-ttu-id="0893d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0893d-119">Name</span></span>       | <span data-ttu-id="0893d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0893d-120">Type</span></span> | <span data-ttu-id="0893d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0893d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0893d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0893d-122">Authorization</span></span>  | <span data-ttu-id="0893d-123">string</span><span class="sxs-lookup"><span data-stu-id="0893d-123">string</span></span>  | <span data-ttu-id="0893d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0893d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0893d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0893d-126">Content-Type</span></span>  | <span data-ttu-id="0893d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0893d-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0893d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0893d-128">Request body</span></span>
<span data-ttu-id="0893d-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0893d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0893d-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0893d-130">Parameter</span></span>    | <span data-ttu-id="0893d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0893d-131">Type</span></span>   |<span data-ttu-id="0893d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0893d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0893d-133">groupIds</span><span class="sxs-lookup"><span data-stu-id="0893d-133">groupIds</span></span>|<span data-ttu-id="0893d-134">String</span><span class="sxs-lookup"><span data-stu-id="0893d-134">String</span></span>|<span data-ttu-id="0893d-p104">Uma coleção que contém as IDs de objetos dos grupos em que se deve verificar a associação. Até 20 grupos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="0893d-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="0893d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0893d-137">Response</span></span>

<span data-ttu-id="0893d-138">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0893d-138">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0893d-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0893d-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0893d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0893d-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="0893d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0893d-141">Response</span></span>
<span data-ttu-id="0893d-p105">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0893d-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
