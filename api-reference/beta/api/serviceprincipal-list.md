---
title: Lista servicePrincipals
description: Recupere uma lista de objetos servicePrincipal.
localization_priority: Normal
ms.openlocfilehash: d7e0a9a34ac0ab7a166c40336671ec4d0a89ddd6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837608"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="61281-103">Lista servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="61281-103">List servicePrincipals</span></span>

> <span data-ttu-id="61281-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="61281-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61281-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61281-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61281-106">Recupere uma lista de objetos servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="61281-106">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="61281-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="61281-107">Permissions</span></span>

<span data-ttu-id="61281-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61281-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="61281-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61281-110">Permission type</span></span>      | <span data-ttu-id="61281-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61281-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61281-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61281-112">Delegated (work or school account)</span></span> | <span data-ttu-id="61281-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="61281-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="61281-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61281-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61281-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61281-115">Not supported.</span></span>    |
|<span data-ttu-id="61281-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61281-116">Application</span></span> | <span data-ttu-id="61281-117">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="61281-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61281-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61281-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="61281-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61281-119">Optional query parameters</span></span>

<span data-ttu-id="61281-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61281-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61281-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61281-121">Request headers</span></span>
| <span data-ttu-id="61281-122">Nome</span><span class="sxs-lookup"><span data-stu-id="61281-122">Name</span></span> | <span data-ttu-id="61281-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="61281-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="61281-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="61281-124">Authorization</span></span>  | <span data-ttu-id="61281-125">string</span><span class="sxs-lookup"><span data-stu-id="61281-125">string</span></span>  | <span data-ttu-id="61281-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61281-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61281-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61281-128">Request body</span></span>

<span data-ttu-id="61281-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61281-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61281-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="61281-130">Response</span></span>

<span data-ttu-id="61281-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61281-131">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61281-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61281-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="61281-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61281-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="61281-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="61281-134">Response</span></span>

<span data-ttu-id="61281-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61281-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal",
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
<!-- {
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
