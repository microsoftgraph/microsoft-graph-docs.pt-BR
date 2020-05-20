---
title: 'servicePrincipalName: checkMemberObjects'
description: Verifique se há associação em uma lista de grupos, funções de diretório ou unidades administrativas para o objeto de princípio de serviço especificado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad8f8b6a4b295964fad5332f86b942bfb9c8373f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289840"
---
# <a name="serviceprincipal-checkmemberobjects"></a><span data-ttu-id="aaa26-103">servicePrincipalName: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="aaa26-103">servicePrincipal: checkMemberObjects</span></span>

<span data-ttu-id="aaa26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaa26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aaa26-105">Verifique se há associação em uma lista de grupos, funções de diretório ou unidades administrativas para o objeto [servicePrincipalName](../resources/serviceprincipal.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="aaa26-105">Check for membership in a list of groups, directory roles, or administrative units for the specified [servicePrincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="aaa26-106">Este método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="aaa26-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaa26-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="aaa26-107">Permissions</span></span>

<span data-ttu-id="aaa26-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaa26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aaa26-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aaa26-110">Permission type</span></span>                        | <span data-ttu-id="aaa26-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aaa26-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aaa26-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aaa26-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="aaa26-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aaa26-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>|
| <span data-ttu-id="aaa26-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aaa26-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaa26-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaa26-115">Not supported.</span></span> |
| <span data-ttu-id="aaa26-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aaa26-116">Application</span></span>                            | <span data-ttu-id="aaa26-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaa26-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaa26-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aaa26-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="aaa26-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aaa26-119">Request headers</span></span>
| <span data-ttu-id="aaa26-120">Nome</span><span class="sxs-lookup"><span data-stu-id="aaa26-120">Name</span></span>       | <span data-ttu-id="aaa26-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaa26-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="aaa26-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aaa26-122">Authorization</span></span> | <span data-ttu-id="aaa26-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aaa26-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="aaa26-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aaa26-125">Content-Type</span></span> | <span data-ttu-id="aaa26-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aaa26-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aaa26-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aaa26-128">Request body</span></span>

<span data-ttu-id="aaa26-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aaa26-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aaa26-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aaa26-130">Parameter</span></span>    | <span data-ttu-id="aaa26-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aaa26-131">Type</span></span>        | <span data-ttu-id="aaa26-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaa26-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aaa26-133">ids</span><span class="sxs-lookup"><span data-stu-id="aaa26-133">ids</span></span>|<span data-ttu-id="aaa26-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aaa26-134">String collection</span></span>|<span data-ttu-id="aaa26-135">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório, unidades administrativas ou IDs RoleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="aaa26-135">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="aaa26-136">Até 20 objetos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="aaa26-136">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="aaa26-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaa26-137">Response</span></span>

<span data-ttu-id="aaa26-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aaa26-138">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aaa26-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aaa26-139">Examples</span></span>

<span data-ttu-id="aaa26-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="aaa26-140">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="aaa26-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aaa26-141">Request</span></span>

<span data-ttu-id="aaa26-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aaa26-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/checkMemberObjects
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

### <a name="response"></a><span data-ttu-id="aaa26-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaa26-143">Response</span></span>

<span data-ttu-id="aaa26-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aaa26-144">The following is an example of the response.</span></span> 

> <span data-ttu-id="aaa26-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aaa26-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
