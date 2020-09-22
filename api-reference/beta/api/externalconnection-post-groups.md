---
title: Criar um
description: Criar um novo objeto de objeto externo.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: fb836591b86972144f3ff632f807f7e1d4c0e82c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193818"
---
# <a name="create-externalgroup"></a><span data-ttu-id="c796f-103">Criar um</span><span class="sxs-lookup"><span data-stu-id="c796f-103">Create externalGroup</span></span>

<span data-ttu-id="c796f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c796f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c796f-105">Criar um novo objeto de objeto [externo](../resources/externalgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="c796f-105">Create a new [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c796f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c796f-106">Permissions</span></span>

<span data-ttu-id="c796f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c796f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c796f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c796f-109">Permission type</span></span>                        | <span data-ttu-id="c796f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c796f-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c796f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c796f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c796f-112">Incompatível</span><span class="sxs-lookup"><span data-stu-id="c796f-112">Not supported</span></span>                               |
| <span data-ttu-id="c796f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c796f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c796f-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c796f-114">Not supported</span></span>                               |
| <span data-ttu-id="c796f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c796f-115">Application</span></span>                            | <span data-ttu-id="c796f-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c796f-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="c796f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c796f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionId}/groups
```

## <a name="request-headers"></a><span data-ttu-id="c796f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c796f-118">Request headers</span></span>

| <span data-ttu-id="c796f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c796f-119">Name</span></span>          | <span data-ttu-id="c796f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c796f-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="c796f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c796f-121">Authorization</span></span> | <span data-ttu-id="c796f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c796f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="c796f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c796f-124">Content-Type</span></span>  | <span data-ttu-id="c796f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c796f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c796f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c796f-127">Request body</span></span>

<span data-ttu-id="c796f-128">No corpo da solicitação, forneça uma representação JSON do objeto de objeto [externo](../resources/externalgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="c796f-128">In the request body, supply a JSON representation of the [externalGroup](../resources/externalgroup.md) object.</span></span>

<span data-ttu-id="c796f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o [myexternalsource](../resources/externalgroup.md).</span><span class="sxs-lookup"><span data-stu-id="c796f-129">The following table shows the properties that are required when you create the [externalGroup](../resources/externalgroup.md).</span></span>

| <span data-ttu-id="c796f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c796f-130">Property</span></span>    | <span data-ttu-id="c796f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c796f-131">Type</span></span>   | <span data-ttu-id="c796f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c796f-132">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c796f-133">id</span><span class="sxs-lookup"><span data-stu-id="c796f-133">id</span></span>          | <span data-ttu-id="c796f-134">String</span><span class="sxs-lookup"><span data-stu-id="c796f-134">String</span></span> | <span data-ttu-id="c796f-135">A identificação exclusiva do grupo externo em uma conexão.</span><span class="sxs-lookup"><span data-stu-id="c796f-135">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="c796f-136">Ele deve ser alfanumérico e até 128 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="c796f-136">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="c796f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c796f-137">displayName</span></span> | <span data-ttu-id="c796f-138">String</span><span class="sxs-lookup"><span data-stu-id="c796f-138">String</span></span> | <span data-ttu-id="c796f-139">O nome amigável do grupo externo.</span><span class="sxs-lookup"><span data-stu-id="c796f-139">The friendly name of the external group.</span></span> <span data-ttu-id="c796f-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c796f-140">Optional.</span></span>                                                                      |
| <span data-ttu-id="c796f-141">description</span><span class="sxs-lookup"><span data-stu-id="c796f-141">description</span></span> | <span data-ttu-id="c796f-142">String</span><span class="sxs-lookup"><span data-stu-id="c796f-142">String</span></span> | <span data-ttu-id="c796f-143">A descrição do grupo externo.</span><span class="sxs-lookup"><span data-stu-id="c796f-143">The description of the external group.</span></span> <span data-ttu-id="c796f-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c796f-144">Optional.</span></span>                                                                         |

## <a name="response"></a><span data-ttu-id="c796f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c796f-145">Response</span></span>

<span data-ttu-id="c796f-146">Se bem-sucedido, este método retorna um `201 Created` código de resposta e [externalGroup](../resources/externalgroup.md) um objeto de myFormat no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c796f-146">If successful, this method returns a `201 Created` response code and an [externalGroup](../resources/externalgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c796f-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c796f-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c796f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c796f-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_connection"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="c796f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c796f-149">Response</span></span>

<span data-ttu-id="c796f-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c796f-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroup"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
