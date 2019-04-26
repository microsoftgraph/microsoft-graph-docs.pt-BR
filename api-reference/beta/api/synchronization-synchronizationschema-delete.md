---
title: Excluir synchronizationSchema
description: Exclui o esquema personalizado e redefine o esquema para a configuração padrão. Se o esquema for excluído no contexto do modelo, ele redefinirá o esquema como o padrão associado ao modelo do `factoryTag`.
localization_priority: Normal
ms.openlocfilehash: 0871de0ba5b48784e47fd5cc8d3ac890ab23748b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330610"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="a6b80-104">Excluir synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="a6b80-104">Delete synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6b80-105">Exclui o esquema personalizado e redefine o esquema para a configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="a6b80-105">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="a6b80-106">Se o esquema for excluído no contexto do modelo, ele redefinirá o esquema como o padrão associado ao modelo do `factoryTag`.</span><span class="sxs-lookup"><span data-stu-id="a6b80-106">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6b80-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6b80-107">Permissions</span></span>
<span data-ttu-id="a6b80-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6b80-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6b80-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6b80-110">Permission type</span></span>                        | <span data-ttu-id="a6b80-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6b80-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6b80-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6b80-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="a6b80-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6b80-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a6b80-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6b80-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a6b80-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6b80-115">Not supported.</span></span>|
|<span data-ttu-id="a6b80-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6b80-116">Application</span></span>                            |<span data-ttu-id="a6b80-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6b80-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="a6b80-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6b80-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="a6b80-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b80-119">Request headers</span></span>

| <span data-ttu-id="a6b80-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a6b80-120">Name</span></span>           | <span data-ttu-id="a6b80-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6b80-121">Type</span></span>    | <span data-ttu-id="a6b80-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6b80-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a6b80-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6b80-123">Authorization</span></span>  | <span data-ttu-id="a6b80-124">string</span><span class="sxs-lookup"><span data-stu-id="a6b80-124">string</span></span>  | <span data-ttu-id="a6b80-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6b80-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6b80-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b80-127">Request body</span></span>

<span data-ttu-id="a6b80-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6b80-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6b80-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6b80-129">Response</span></span>

<span data-ttu-id="a6b80-130">Se tiver êxito, este método retornará um código de resposta `201 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a6b80-130">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="a6b80-131">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6b80-131">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6b80-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6b80-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a6b80-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b80-133">Request</span></span>
<span data-ttu-id="a6b80-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6b80-134">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="a6b80-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6b80-135">Response</span></span>
<span data-ttu-id="a6b80-136">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="a6b80-136">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
