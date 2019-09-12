---
title: 'dispositivo: checkMemberObjects'
description: Verifique se há associação em uma lista de grupos, funções de diretório ou unidades administrativas para o objeto de dispositivo especificado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 094b3734babd69aa46e8c703ebddb592ff46307d
ms.sourcegitcommit: 4ce5060cddfa92cc282321bd9cfbf0a39de51aae
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2019
ms.locfileid: "36853837"
---
# <a name="device-checkmemberobjects"></a><span data-ttu-id="b5ceb-103">dispositivo: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="b5ceb-103">device: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5ceb-104">Verifique se há associação em uma lista de grupos ou unidades administrativas para o objeto de dispositivo especificado.</span><span class="sxs-lookup"><span data-stu-id="b5ceb-104">Check for membership in a list of groups or administrative units for the specified device object.</span></span> <span data-ttu-id="b5ceb-105">Este método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="b5ceb-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5ceb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5ceb-106">Permissions</span></span>

<span data-ttu-id="b5ceb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5ceb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5ceb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5ceb-109">Permission type</span></span>                        | <span data-ttu-id="b5ceb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5ceb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b5ceb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5ceb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5ceb-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b5ceb-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="b5ceb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5ceb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5ceb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5ceb-114">Not supported.</span></span> |
| <span data-ttu-id="b5ceb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5ceb-115">Application</span></span>                            | <span data-ttu-id="b5ceb-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5ceb-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5ceb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5ceb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /devices/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="b5ceb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5ceb-118">Request headers</span></span>

| <span data-ttu-id="b5ceb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b5ceb-119">Name</span></span>          | <span data-ttu-id="b5ceb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5ceb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b5ceb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5ceb-121">Authorization</span></span> | <span data-ttu-id="b5ceb-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b5ceb-122">Bearer {token}</span></span> |
| <span data-ttu-id="b5ceb-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5ceb-123">Content-Type</span></span>  | <span data-ttu-id="b5ceb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b5ceb-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5ceb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5ceb-125">Request body</span></span>

<span data-ttu-id="b5ceb-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5ceb-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b5ceb-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b5ceb-127">Parameter</span></span>    | <span data-ttu-id="b5ceb-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5ceb-128">Type</span></span>        | <span data-ttu-id="b5ceb-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5ceb-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b5ceb-130">ids</span><span class="sxs-lookup"><span data-stu-id="b5ceb-130">ids</span></span> | <span data-ttu-id="b5ceb-131">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ceb-131">String collection</span></span> | <span data-ttu-id="b5ceb-132">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório, unidades administrativas ou IDs RoleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="b5ceb-132">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="b5ceb-133">Até 20 objetos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="b5ceb-133">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="b5ceb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5ceb-134">Response</span></span>

<span data-ttu-id="b5ceb-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5ceb-135">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5ceb-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b5ceb-136">Examples</span></span>

<span data-ttu-id="b5ceb-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b5ceb-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b5ceb-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5ceb-138">Request</span></span>

<span data-ttu-id="b5ceb-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5ceb-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "device_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/devices/{id}/checkMemberObjects
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

### <a name="response"></a><span data-ttu-id="b5ceb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5ceb-140">Response</span></span>

<span data-ttu-id="b5ceb-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5ceb-141">The following is an example of the response.</span></span> 

> <span data-ttu-id="b5ceb-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5ceb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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