---
title: Obter servicePrincipal
description: Recupere as propriedades e relações do objeto serviceprincipal.
ms.openlocfilehash: 903bec11787b4b5acc5da688f7b73bf2bbd76262
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040626"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="4102d-103">Obter servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="4102d-103">Get servicePrincipal</span></span>

> <span data-ttu-id="4102d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4102d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4102d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4102d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4102d-106">Recupere as propriedades e relações do objeto serviceprincipal.</span><span class="sxs-lookup"><span data-stu-id="4102d-106">Retrieve the properties and relationships of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4102d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="4102d-107">Permissions</span></span>
<span data-ttu-id="4102d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4102d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4102d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4102d-110">Permission type</span></span>      | <span data-ttu-id="4102d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4102d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4102d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4102d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4102d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4102d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4102d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4102d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4102d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4102d-115">Not supported.</span></span>    |
|<span data-ttu-id="4102d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4102d-116">Application</span></span> | <span data-ttu-id="4102d-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4102d-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4102d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4102d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4102d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4102d-119">Optional query parameters</span></span>
<span data-ttu-id="4102d-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4102d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4102d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4102d-121">Request headers</span></span>
| <span data-ttu-id="4102d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4102d-122">Name</span></span>       | <span data-ttu-id="4102d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4102d-123">Type</span></span> | <span data-ttu-id="4102d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4102d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4102d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4102d-125">Authorization</span></span>  | <span data-ttu-id="4102d-126">string</span><span class="sxs-lookup"><span data-stu-id="4102d-126">string</span></span>  | <span data-ttu-id="4102d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4102d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4102d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4102d-129">Request body</span></span>
<span data-ttu-id="4102d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4102d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4102d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4102d-131">Response</span></span>

<span data-ttu-id="4102d-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4102d-132">If successful, this method returns a `200 OK` response code and [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4102d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4102d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4102d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4102d-134">Request</span></span>
<span data-ttu-id="4102d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4102d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="4102d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4102d-136">Response</span></span>
<span data-ttu-id="4102d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4102d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->