---
title: Excluir synchronizationSchema
description: Exclui o esquema personalizado e redefine o esquema para a configuração padrão. Se o esquema for excluído no contexto do modelo, ele redefine o esquema para o padrão de um associado do modelo `factoryTag`.
ms.openlocfilehash: 81c1a918b10e8f4553b3e99312f20bb538bfbe4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039151"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="c96e7-104">Excluir synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="c96e7-104">Delete synchronizationSchema</span></span>

> <span data-ttu-id="c96e7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c96e7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c96e7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c96e7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c96e7-107">Exclui o esquema personalizado e redefine o esquema para a configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="c96e7-107">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="c96e7-108">Se o esquema for excluído no contexto do modelo, ele redefine o esquema para o padrão de um associado do modelo `factoryTag`.</span><span class="sxs-lookup"><span data-stu-id="c96e7-108">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="c96e7-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="c96e7-109">Permissions</span></span>
<span data-ttu-id="c96e7-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c96e7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c96e7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c96e7-112">Permission type</span></span>                        | <span data-ttu-id="c96e7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c96e7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c96e7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c96e7-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="c96e7-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c96e7-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c96e7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c96e7-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c96e7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c96e7-117">Not supported.</span></span>|
|<span data-ttu-id="c96e7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c96e7-118">Application</span></span>                            |<span data-ttu-id="c96e7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c96e7-119">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="c96e7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c96e7-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="c96e7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c96e7-121">Request headers</span></span>

| <span data-ttu-id="c96e7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c96e7-122">Name</span></span>           | <span data-ttu-id="c96e7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c96e7-123">Type</span></span>    | <span data-ttu-id="c96e7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c96e7-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c96e7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c96e7-125">Authorization</span></span>  | <span data-ttu-id="c96e7-126">string</span><span class="sxs-lookup"><span data-stu-id="c96e7-126">string</span></span>  | <span data-ttu-id="c96e7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c96e7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c96e7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c96e7-129">Request body</span></span>

<span data-ttu-id="c96e7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c96e7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c96e7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c96e7-131">Response</span></span>

<span data-ttu-id="c96e7-132">Se tiver êxito, este método retornará um código de resposta `201 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c96e7-132">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="c96e7-133">Ele não retornará nada no corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c96e7-133">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="c96e7-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c96e7-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c96e7-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c96e7-135">Request</span></span>
<span data-ttu-id="c96e7-136">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c96e7-136">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="c96e7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c96e7-137">Response</span></span>
<span data-ttu-id="c96e7-138">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c96e7-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->