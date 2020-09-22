---
title: Criar administrativeUnit
description: Use esta API para criar um novo administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6470e1a64b337cd885d5d7cd7a5f728ba9d7a5f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020196"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="15744-103">Criar administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="15744-103">Create administrativeUnit</span></span>

<span data-ttu-id="15744-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15744-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15744-105">Use esta API para criar um novo [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="15744-105">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="15744-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="15744-106">Permissions</span></span>
<span data-ttu-id="15744-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15744-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="15744-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15744-109">Permission type</span></span>      | <span data-ttu-id="15744-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15744-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15744-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15744-111">Delegated (work or school account)</span></span> | <span data-ttu-id="15744-112">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="15744-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="15744-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15744-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15744-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15744-114">Not supported.</span></span>    |
|<span data-ttu-id="15744-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15744-115">Application</span></span> | <span data-ttu-id="15744-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15744-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15744-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15744-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="15744-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15744-118">Request headers</span></span>
| <span data-ttu-id="15744-119">Nome</span><span class="sxs-lookup"><span data-stu-id="15744-119">Name</span></span>      |<span data-ttu-id="15744-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="15744-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="15744-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="15744-121">Authorization</span></span>  | <span data-ttu-id="15744-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15744-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15744-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="15744-124">Content-type</span></span> | <span data-ttu-id="15744-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15744-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15744-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15744-127">Request body</span></span>
<span data-ttu-id="15744-128">No corpo da solicitação, forneça uma representação JSON de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="15744-128">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="15744-129">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à unidade administrativa ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="15744-129">Because the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="15744-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="15744-130">Response</span></span>

<span data-ttu-id="15744-131">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15744-131">If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15744-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15744-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="15744-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15744-133">Request</span></span>

<span data-ttu-id="15744-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="15744-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```

---

<span data-ttu-id="15744-135">No corpo da solicitação, forneça uma representação JSON de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="15744-135">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="15744-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="15744-136">Response</span></span>

<span data-ttu-id="15744-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15744-137">The following is an example of the response.</span></span> 
> <span data-ttu-id="15744-138">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="15744-138">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="15744-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15744-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 172

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#administrativeUnits/$entity",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f",
    "deletedDateTime": null,
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```

## <a name="see-also"></a><span data-ttu-id="15744-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="15744-140">See also</span></span>

- [<span data-ttu-id="15744-141">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="15744-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="15744-142">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="15744-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
