---
title: 'servicePrincipalName: checkMemberObjects'
description: Verifique se há associação em uma lista de grupos, funções de diretório ou unidades administrativas para o objeto de princípio de serviço especificado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f0bcc7dd5c32ebe27e55169a8170069335607444
ms.sourcegitcommit: 4ce5060cddfa92cc282321bd9cfbf0a39de51aae
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2019
ms.locfileid: "36853843"
---
# <a name="serviceprincipal-checkmemberobjects"></a><span data-ttu-id="20620-103">servicePrincipalName: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="20620-103">servicePrincipal: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20620-104">Verifique se há associação em uma lista de grupos, funções de diretório ou unidades administrativas para o objeto de princípio de serviço especificado.</span><span class="sxs-lookup"><span data-stu-id="20620-104">Check for membership in a list of groups, directory roles, or administrative units for the specified service principle object.</span></span> <span data-ttu-id="20620-105">Este método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="20620-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="20620-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20620-106">Permissions</span></span>

<span data-ttu-id="20620-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20620-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20620-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20620-109">Permission type</span></span>                        | <span data-ttu-id="20620-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20620-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="20620-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20620-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="20620-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20620-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>|
| <span data-ttu-id="20620-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20620-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20620-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20620-114">Not supported.</span></span> |
| <span data-ttu-id="20620-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20620-115">Application</span></span>                            | <span data-ttu-id="20620-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20620-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20620-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20620-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="20620-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20620-118">Request headers</span></span>

| <span data-ttu-id="20620-119">Nome</span><span class="sxs-lookup"><span data-stu-id="20620-119">Name</span></span>          | <span data-ttu-id="20620-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="20620-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="20620-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="20620-121">Authorization</span></span> | <span data-ttu-id="20620-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="20620-122">Bearer {token}</span></span> |
| <span data-ttu-id="20620-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="20620-123">Content-Type</span></span>  | <span data-ttu-id="20620-124">application/json</span><span class="sxs-lookup"><span data-stu-id="20620-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="20620-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20620-125">Request body</span></span>

<span data-ttu-id="20620-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20620-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20620-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="20620-127">Parameter</span></span>    | <span data-ttu-id="20620-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="20620-128">Type</span></span>        | <span data-ttu-id="20620-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="20620-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20620-130">ids</span><span class="sxs-lookup"><span data-stu-id="20620-130">ids</span></span>|<span data-ttu-id="20620-131">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="20620-131">String collection</span></span>|<span data-ttu-id="20620-132">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório, unidades administrativas ou IDs RoleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="20620-132">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="20620-133">Até 20 objetos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="20620-133">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="20620-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="20620-134">Response</span></span>

<span data-ttu-id="20620-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20620-135">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20620-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20620-136">Examples</span></span>

<span data-ttu-id="20620-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="20620-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="20620-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20620-138">Request</span></span>

<span data-ttu-id="20620-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20620-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberObjects
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

### <a name="response"></a><span data-ttu-id="20620-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="20620-140">Response</span></span>

<span data-ttu-id="20620-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20620-141">The following is an example of the response.</span></span> 

> <span data-ttu-id="20620-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20620-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "servicePrincipal: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->