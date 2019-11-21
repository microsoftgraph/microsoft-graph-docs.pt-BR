---
title: 'dispositivo: checkMemberObjects'
description: Verifique se há associação em uma lista de grupos ou funções de diretório para o objeto de dispositivo especificado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 536781e0a91a88c600d7478f8d93c10db7e66f42
ms.sourcegitcommit: c25828c596b7e0939fa164a3d7754722943152c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2019
ms.locfileid: "38757297"
---
# <a name="device-checkmemberobjects"></a><span data-ttu-id="8863e-103">dispositivo: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="8863e-103">device: checkMemberObjects</span></span>

<span data-ttu-id="8863e-104">Verifique se há associação em uma lista de grupos ou funções de diretório para o objeto de dispositivo especificado.</span><span class="sxs-lookup"><span data-stu-id="8863e-104">Check for membership in a list of groups or directory roles for the specified device object.</span></span> <span data-ttu-id="8863e-105">Este método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="8863e-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="8863e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8863e-106">Permissions</span></span>

<span data-ttu-id="8863e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8863e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8863e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8863e-109">Permission type</span></span>                        | <span data-ttu-id="8863e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8863e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8863e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8863e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8863e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8863e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="8863e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8863e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8863e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8863e-114">Not supported.</span></span> |
| <span data-ttu-id="8863e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8863e-115">Application</span></span>                            | <span data-ttu-id="8863e-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8863e-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8863e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8863e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /devices/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="8863e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8863e-118">Request headers</span></span>

| <span data-ttu-id="8863e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8863e-119">Name</span></span>          | <span data-ttu-id="8863e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8863e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8863e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8863e-121">Authorization</span></span> | <span data-ttu-id="8863e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8863e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8863e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8863e-124">Content-Type</span></span>  | <span data-ttu-id="8863e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8863e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8863e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8863e-127">Request body</span></span>

<span data-ttu-id="8863e-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8863e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8863e-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8863e-129">Parameter</span></span>    | <span data-ttu-id="8863e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8863e-130">Type</span></span>        | <span data-ttu-id="8863e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8863e-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8863e-132">ids</span><span class="sxs-lookup"><span data-stu-id="8863e-132">ids</span></span> | <span data-ttu-id="8863e-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8863e-133">String collection</span></span> | <span data-ttu-id="8863e-134">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório ou IDs RoleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="8863e-134">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="8863e-135">Você pode especificar até 20 objetos.</span><span class="sxs-lookup"><span data-stu-id="8863e-135">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="8863e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8863e-136">Response</span></span>

<span data-ttu-id="8863e-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8863e-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8863e-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8863e-138">Examples</span></span>

<span data-ttu-id="8863e-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8863e-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8863e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8863e-140">Request</span></span>

<span data-ttu-id="8863e-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8863e-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8863e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="8863e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "device_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/devices/{id}/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8863e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8863e-143">Response</span></span>

<span data-ttu-id="8863e-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8863e-144">The following is an example of the response.</span></span> 

> <span data-ttu-id="8863e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8863e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
