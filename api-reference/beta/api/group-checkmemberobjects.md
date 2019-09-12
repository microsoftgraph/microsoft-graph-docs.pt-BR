---
title: 'Grupo: checkMemberObjects'
description: Verifique se há associação em uma lista de grupos, funções de diretório ou unidades administrativas para o objeto de grupo especificado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38f2a460dc147416604f52d092e4cf2f99cc20c7
ms.sourcegitcommit: 4ce5060cddfa92cc282321bd9cfbf0a39de51aae
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2019
ms.locfileid: "36853838"
---
# <a name="group-checkmemberobjects"></a><span data-ttu-id="08564-103">Grupo: checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="08564-103">group: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08564-104">Verifique se há associação em uma lista de grupos ou unidades administrativas para o grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="08564-104">Check for membership in a list of groups or administrative units for the specified group.</span></span> <span data-ttu-id="08564-105">Este método é transitivo.</span><span class="sxs-lookup"><span data-stu-id="08564-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="08564-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="08564-106">Permissions</span></span>

<span data-ttu-id="08564-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08564-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08564-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08564-109">Permission type</span></span>                        | <span data-ttu-id="08564-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08564-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="08564-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08564-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="08564-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08564-112">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="08564-113">E</span><span class="sxs-lookup"><span data-stu-id="08564-113">And:</span></span><br><ul><li><span data-ttu-id="08564-114">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="08564-114">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li></ul><br><span data-ttu-id="08564-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08564-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="08564-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08564-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08564-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08564-117">Not supported.</span></span> |
| <span data-ttu-id="08564-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08564-118">Application</span></span>                            | <span data-ttu-id="08564-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08564-119">Group.Read.All, Group.ReadWrite.All</span></span><br><span data-ttu-id="08564-120">E</span><span class="sxs-lookup"><span data-stu-id="08564-120">And:</span></span><br><ul><li><span data-ttu-id="08564-121">Se estiver verificando a associação em unidades administrativas: AdministrativeUnit. Read. All, AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="08564-121">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></ul></li><br><span data-ttu-id="08564-122">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08564-122">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08564-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08564-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="08564-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08564-124">Request headers</span></span>

| <span data-ttu-id="08564-125">Nome</span><span class="sxs-lookup"><span data-stu-id="08564-125">Name</span></span>          | <span data-ttu-id="08564-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="08564-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="08564-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="08564-127">Authorization</span></span> | <span data-ttu-id="08564-128">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="08564-128">Bearer {token}</span></span> |
| <span data-ttu-id="08564-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08564-129">Content-Type</span></span>  | <span data-ttu-id="08564-130">application/json</span><span class="sxs-lookup"><span data-stu-id="08564-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="08564-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08564-131">Request body</span></span>

<span data-ttu-id="08564-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08564-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08564-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="08564-133">Parameter</span></span>    | <span data-ttu-id="08564-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="08564-134">Type</span></span>        | <span data-ttu-id="08564-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="08564-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08564-136">ids</span><span class="sxs-lookup"><span data-stu-id="08564-136">ids</span></span>|<span data-ttu-id="08564-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="08564-137">String collection</span></span>| <span data-ttu-id="08564-138">Uma coleção que contém as IDs de objeto dos grupos, funções de diretório, unidades administrativas ou IDs RoleTemplate de funções de diretório, para verificar a associação.</span><span class="sxs-lookup"><span data-stu-id="08564-138">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="08564-139">Até 20 objetos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="08564-139">Up to 20 objects may be specified.</span></span> |

## <a name="response"></a><span data-ttu-id="08564-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="08564-140">Response</span></span>

<span data-ttu-id="08564-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08564-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08564-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="08564-142">Examples</span></span>

<span data-ttu-id="08564-143">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="08564-143">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="08564-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08564-144">Request</span></span>

<span data-ttu-id="08564-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="08564-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberObjects
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

### <a name="response"></a><span data-ttu-id="08564-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="08564-146">Response</span></span>

<span data-ttu-id="08564-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="08564-147">The following is an example of the response.</span></span> 

> <span data-ttu-id="08564-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08564-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->