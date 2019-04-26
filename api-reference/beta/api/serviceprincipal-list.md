---
title: List servicePrincipals
description: Recupere uma lista de objetos servicePrincipal.
localization_priority: Normal
ms.openlocfilehash: 42b98ea6f2fcdf10620a632c8325a80fae61fac0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335861"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="bbf82-103">List servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="bbf82-103">List servicePrincipals</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbf82-104">Recupere uma lista de objetos servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="bbf82-104">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbf82-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbf82-105">Permissions</span></span>

<span data-ttu-id="bbf82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbf82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bbf82-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbf82-108">Permission type</span></span>      | <span data-ttu-id="bbf82-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbf82-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbf82-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbf82-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bbf82-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bbf82-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bbf82-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbf82-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbf82-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbf82-113">Not supported.</span></span>    |
|<span data-ttu-id="bbf82-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbf82-114">Application</span></span> | <span data-ttu-id="bbf82-115">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf82-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbf82-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf82-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bbf82-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bbf82-117">Optional query parameters</span></span>

<span data-ttu-id="bbf82-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bbf82-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbf82-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf82-119">Request headers</span></span>
| <span data-ttu-id="bbf82-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bbf82-120">Name</span></span> | <span data-ttu-id="bbf82-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbf82-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="bbf82-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbf82-122">Authorization</span></span>  | <span data-ttu-id="bbf82-123">string</span><span class="sxs-lookup"><span data-stu-id="bbf82-123">string</span></span>  | <span data-ttu-id="bbf82-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbf82-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbf82-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf82-126">Request body</span></span>

<span data-ttu-id="bbf82-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bbf82-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbf82-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf82-128">Response</span></span>

<span data-ttu-id="bbf82-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos de [servicePrincipalName](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbf82-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbf82-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbf82-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bbf82-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf82-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="bbf82-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf82-132">Response</span></span>

<span data-ttu-id="bbf82-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbf82-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 488

{
  "value": [
    {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
