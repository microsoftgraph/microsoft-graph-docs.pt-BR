---
title: Listar scopedAdministratorOf
description: Recupere uma lista de scopedRoleMembership para o usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c353d2875d069577bda54d42533b8c7d48720aa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329827"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="58e37-103">Listar scopedAdministratorOf</span><span class="sxs-lookup"><span data-stu-id="58e37-103">List scopedAdministratorOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58e37-104">Recupere uma lista de [scopedRoleMembership](../resources/scopedrolemembership.md) para o usuário.</span><span class="sxs-lookup"><span data-stu-id="58e37-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="58e37-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="58e37-105">Permissions</span></span>
<span data-ttu-id="58e37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58e37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="58e37-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58e37-108">Permission type</span></span>      | <span data-ttu-id="58e37-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58e37-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58e37-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58e37-110">Delegated (work or school account)</span></span> | <span data-ttu-id="58e37-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="58e37-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="58e37-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58e37-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58e37-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58e37-113">Not supported.</span></span>    |
|<span data-ttu-id="58e37-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58e37-114">Application</span></span> | <span data-ttu-id="58e37-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e37-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58e37-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58e37-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedAdministratorOf
GET /users/{id}/scopedAdministratorOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="58e37-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58e37-117">Optional query parameters</span></span>
<span data-ttu-id="58e37-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="58e37-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58e37-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58e37-119">Request headers</span></span>
| <span data-ttu-id="58e37-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58e37-120">Header</span></span>       | <span data-ttu-id="58e37-121">Valor</span><span class="sxs-lookup"><span data-stu-id="58e37-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="58e37-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="58e37-122">Authorization</span></span>  | <span data-ttu-id="58e37-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58e37-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="58e37-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58e37-125">Request body</span></span>
<span data-ttu-id="58e37-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58e37-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58e37-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="58e37-127">Response</span></span>

<span data-ttu-id="58e37-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58e37-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58e37-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58e37-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58e37-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58e37-130">Request</span></span>
<span data-ttu-id="58e37-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58e37-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```http
GET https://graph.microsoft.com/beta/me/scopedAdministratorOf
```
##### <a name="response"></a><span data-ttu-id="58e37-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="58e37-132">Response</span></span>
<span data-ttu-id="58e37-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58e37-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      },
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedAdministratorOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
