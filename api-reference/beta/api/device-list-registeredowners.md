---
title: Listar registeredOwners
description: Recupera uma lista de usuários que são proprietários registrados do dispositivo. Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal. O proprietário registrado é definido no momento do registro. Atualmente, só pode haver um proprietário.
ms.openlocfilehash: 9b2acee14598c631c7f782391cb22a7917685e02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037792"
---
# <a name="list-registeredowners"></a><span data-ttu-id="7837b-106">Listar registeredOwners</span><span class="sxs-lookup"><span data-stu-id="7837b-106">List registeredOwners</span></span>

> <span data-ttu-id="7837b-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7837b-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7837b-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7837b-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7837b-109">Recupera uma lista de usuários que são proprietários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7837b-109">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="7837b-110">Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal.</span><span class="sxs-lookup"><span data-stu-id="7837b-110">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="7837b-111">O proprietário registrado é definido no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="7837b-111">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="7837b-112">Atualmente, só pode haver um proprietário.</span><span class="sxs-lookup"><span data-stu-id="7837b-112">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="7837b-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="7837b-113">Permissions</span></span>

<span data-ttu-id="7837b-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7837b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7837b-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7837b-116">Permission type</span></span>      | <span data-ttu-id="7837b-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7837b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7837b-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7837b-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7837b-119">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7837b-119">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7837b-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7837b-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7837b-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7837b-121">Not supported.</span></span>    |
|<span data-ttu-id="7837b-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7837b-122">Application</span></span> | <span data-ttu-id="7837b-123">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7837b-123">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7837b-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7837b-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="7837b-125">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="7837b-125">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="7837b-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7837b-126">Optional query parameters</span></span>
<span data-ttu-id="7837b-127">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7837b-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7837b-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7837b-128">Request headers</span></span>
| <span data-ttu-id="7837b-129">Nome</span><span class="sxs-lookup"><span data-stu-id="7837b-129">Name</span></span>       | <span data-ttu-id="7837b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7837b-130">Type</span></span> | <span data-ttu-id="7837b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7837b-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7837b-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="7837b-132">Authorization</span></span>  | <span data-ttu-id="7837b-133">string</span><span class="sxs-lookup"><span data-stu-id="7837b-133">string</span></span>  | <span data-ttu-id="7837b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7837b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7837b-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7837b-136">Request body</span></span>
<span data-ttu-id="7837b-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7837b-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7837b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7837b-138">Response</span></span>

<span data-ttu-id="7837b-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7837b-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7837b-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7837b-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7837b-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7837b-141">Request</span></span>
<span data-ttu-id="7837b-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7837b-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="7837b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7837b-143">Response</span></span>
<span data-ttu-id="7837b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7837b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->