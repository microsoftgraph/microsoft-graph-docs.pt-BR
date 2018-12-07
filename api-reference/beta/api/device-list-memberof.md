---
title: Grupos de dispositivos de lista
description: Obtenha os grupos dos quais este dispositivo é um membro direto. Esta operação não é transitiva.
ms.openlocfilehash: fae373a896a2fc048257a5dc6cd9eb07a85ec677
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184466"
---
# <a name="list-device-groups"></a><span data-ttu-id="c22d4-104">Grupos de dispositivos de lista</span><span class="sxs-lookup"><span data-stu-id="c22d4-104">List device groups</span></span>

> <span data-ttu-id="c22d4-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c22d4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c22d4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c22d4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c22d4-107">Obtenha os grupos dos quais este dispositivo é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="c22d4-107">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="c22d4-108">Esta operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="c22d4-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="c22d4-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c22d4-109">Permissions</span></span>

<span data-ttu-id="c22d4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c22d4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c22d4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c22d4-112">Permission type</span></span>      | <span data-ttu-id="c22d4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c22d4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c22d4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c22d4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c22d4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c22d4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c22d4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c22d4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c22d4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c22d4-117">Not supported.</span></span>    |
|<span data-ttu-id="c22d4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c22d4-118">Application</span></span> | <span data-ttu-id="c22d4-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c22d4-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c22d4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c22d4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c22d4-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c22d4-121">Optional query parameters</span></span>
<span data-ttu-id="c22d4-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c22d4-122">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c22d4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c22d4-123">Request headers</span></span>
| <span data-ttu-id="c22d4-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c22d4-124">Header</span></span>       | <span data-ttu-id="c22d4-125">Valor</span><span class="sxs-lookup"><span data-stu-id="c22d4-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c22d4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c22d4-126">Authorization</span></span>  | <span data-ttu-id="c22d4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c22d4-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c22d4-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c22d4-129">Accept</span></span>  | <span data-ttu-id="c22d4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c22d4-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c22d4-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c22d4-131">Request body</span></span>
<span data-ttu-id="c22d4-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c22d4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c22d4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c22d4-133">Response</span></span>

<span data-ttu-id="c22d4-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c22d4-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c22d4-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c22d4-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="c22d4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c22d4-136">Request</span></span>

<span data-ttu-id="c22d4-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c22d4-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="c22d4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c22d4-138">Response</span></span>
<span data-ttu-id="c22d4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c22d4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
}-->S