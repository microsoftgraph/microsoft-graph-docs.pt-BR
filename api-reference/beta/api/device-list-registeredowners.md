---
title: Listar registeredOwners
description: Recupera uma lista de usuários que são proprietários registrados do dispositivo. Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal. O proprietário registrado é definido no momento do registro. Atualmente, só pode haver um proprietário.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b9020c4fad74990a18023bdddd63ae3bd050998
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455272"
---
# <a name="list-registeredowners"></a><span data-ttu-id="81cdc-106">Listar registeredOwners</span><span class="sxs-lookup"><span data-stu-id="81cdc-106">List registeredOwners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81cdc-107">Recupera uma lista de usuários que são proprietários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81cdc-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="81cdc-108">Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal.</span><span class="sxs-lookup"><span data-stu-id="81cdc-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="81cdc-109">O proprietário registrado é definido no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="81cdc-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="81cdc-110">Atualmente, só pode haver um proprietário.</span><span class="sxs-lookup"><span data-stu-id="81cdc-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="81cdc-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="81cdc-111">Permissions</span></span>

<span data-ttu-id="81cdc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81cdc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81cdc-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81cdc-114">Permission type</span></span>      | <span data-ttu-id="81cdc-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81cdc-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81cdc-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81cdc-116">Delegated (work or school account)</span></span> | <span data-ttu-id="81cdc-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81cdc-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81cdc-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81cdc-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81cdc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81cdc-119">Not supported.</span></span>    |
|<span data-ttu-id="81cdc-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81cdc-120">Application</span></span> | <span data-ttu-id="81cdc-121">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81cdc-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81cdc-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81cdc-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="81cdc-123">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="81cdc-123">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="81cdc-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81cdc-124">Optional query parameters</span></span>
<span data-ttu-id="81cdc-125">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="81cdc-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="81cdc-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81cdc-126">Request headers</span></span>
| <span data-ttu-id="81cdc-127">Nome</span><span class="sxs-lookup"><span data-stu-id="81cdc-127">Name</span></span>       | <span data-ttu-id="81cdc-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="81cdc-128">Type</span></span> | <span data-ttu-id="81cdc-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="81cdc-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="81cdc-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="81cdc-130">Authorization</span></span>  | <span data-ttu-id="81cdc-131">string</span><span class="sxs-lookup"><span data-stu-id="81cdc-131">string</span></span>  | <span data-ttu-id="81cdc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81cdc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81cdc-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81cdc-134">Request body</span></span>
<span data-ttu-id="81cdc-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81cdc-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81cdc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="81cdc-136">Response</span></span>

<span data-ttu-id="81cdc-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81cdc-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="81cdc-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81cdc-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81cdc-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81cdc-139">Request</span></span>
<span data-ttu-id="81cdc-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81cdc-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="81cdc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="81cdc-141">Response</span></span>
<span data-ttu-id="81cdc-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81cdc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-list-registeredowners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
