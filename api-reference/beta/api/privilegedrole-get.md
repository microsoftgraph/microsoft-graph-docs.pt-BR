---
title: Get privilegedRole
description: 'Recupere as propriedades e os relacionamentos do objeto privilegedRole. '
localization_priority: Normal
ms.openlocfilehash: 54fbf8bab03003a03f607bc540414190573a6158
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538572"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="f21f1-103">Get privilegedRole</span><span class="sxs-lookup"><span data-stu-id="f21f1-103">Get privilegedRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f21f1-104">Recupere as propriedades e os relacionamentos do objeto [privilegedRole](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="f21f1-104">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f21f1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f21f1-105">Permissions</span></span>
<span data-ttu-id="f21f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f21f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f21f1-108">O solicitante precisa ter uma das seguintes funções: administrador de _função privilegiada_, _administrador global_, _administrador de segurança_ou _leitor de segurança_.</span><span class="sxs-lookup"><span data-stu-id="f21f1-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="f21f1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f21f1-109">Permission type</span></span>      | <span data-ttu-id="f21f1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f21f1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f21f1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f21f1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f21f1-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f21f1-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f21f1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f21f1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f21f1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f21f1-114">Not supported.</span></span>    |
|<span data-ttu-id="f21f1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f21f1-115">Application</span></span> | <span data-ttu-id="f21f1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f21f1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f21f1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f21f1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f21f1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f21f1-118">Optional query parameters</span></span>
<span data-ttu-id="f21f1-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f21f1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f21f1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f21f1-120">Request headers</span></span>
| <span data-ttu-id="f21f1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f21f1-121">Name</span></span>      |<span data-ttu-id="f21f1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f21f1-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f21f1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f21f1-123">Authorization</span></span>  | <span data-ttu-id="f21f1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f21f1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f21f1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f21f1-126">Request body</span></span>
<span data-ttu-id="f21f1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f21f1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f21f1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f21f1-128">Response</span></span>

<span data-ttu-id="f21f1-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedRole](../resources/privilegedrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f21f1-129">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="f21f1-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="f21f1-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f21f1-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="f21f1-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="f21f1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f21f1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f21f1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f21f1-133">Request</span></span>
<span data-ttu-id="f21f1-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f21f1-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="f21f1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f21f1-135">Response</span></span>
<span data-ttu-id="f21f1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f21f1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
