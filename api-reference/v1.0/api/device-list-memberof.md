---
title: Grupos de dispositivos de lista
description: Obtenha os grupos dos quais este dispositivo é um membro direto. Esta operação não é transitiva.
author: tfitzmac
ms.openlocfilehash: a73bc3c2db80169634f8217418026c0e5c34a033
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306920"
---
# <a name="list-device-groups"></a><span data-ttu-id="05120-104">Grupos de dispositivos de lista</span><span class="sxs-lookup"><span data-stu-id="05120-104">List device groups</span></span>

<span data-ttu-id="05120-105">Obtenha os grupos dos quais este dispositivo é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="05120-105">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="05120-106">Esta operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="05120-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="05120-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="05120-107">Permissions</span></span>

<span data-ttu-id="05120-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05120-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05120-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05120-110">Permission type</span></span>      | <span data-ttu-id="05120-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05120-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05120-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05120-112">Delegated (work or school account)</span></span> | <span data-ttu-id="05120-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05120-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05120-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05120-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05120-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05120-115">Not supported.</span></span>    |
|<span data-ttu-id="05120-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05120-116">Application</span></span> | <span data-ttu-id="05120-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05120-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05120-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05120-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05120-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="05120-119">Optional query parameters</span></span>
<span data-ttu-id="05120-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="05120-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="05120-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05120-121">Request headers</span></span>
| <span data-ttu-id="05120-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05120-122">Header</span></span>       | <span data-ttu-id="05120-123">Valor</span><span class="sxs-lookup"><span data-stu-id="05120-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="05120-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="05120-124">Authorization</span></span>  | <span data-ttu-id="05120-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05120-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="05120-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05120-127">Accept</span></span>  | <span data-ttu-id="05120-128">application/json</span><span class="sxs-lookup"><span data-stu-id="05120-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05120-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05120-129">Request body</span></span>
<span data-ttu-id="05120-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05120-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05120-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="05120-131">Response</span></span>

<span data-ttu-id="05120-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05120-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05120-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05120-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="05120-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05120-134">Request</span></span>

<span data-ttu-id="05120-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05120-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="05120-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="05120-136">Response</span></span>
<span data-ttu-id="05120-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05120-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->