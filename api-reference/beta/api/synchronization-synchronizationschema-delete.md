---
title: Excluir synchronizationSchema
description: Exclui o esquema personalizado e redefine o esquema para a configuração padrão. Se o esquema for excluído no contexto do modelo, ele redefine o esquema para o padrão de um associado do modelo `factoryTag`.
localization_priority: Normal
ms.openlocfilehash: 281911d34355f598f4a3fe57b20c701dde36d4b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855885"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="a54a8-104">Excluir synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="a54a8-104">Delete synchronizationSchema</span></span>

> <span data-ttu-id="a54a8-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a54a8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a54a8-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a54a8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a54a8-107">Exclui o esquema personalizado e redefine o esquema para a configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="a54a8-107">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="a54a8-108">Se o esquema for excluído no contexto do modelo, ele redefine o esquema para o padrão de um associado do modelo `factoryTag`.</span><span class="sxs-lookup"><span data-stu-id="a54a8-108">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a54a8-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="a54a8-109">Permissions</span></span>
<span data-ttu-id="a54a8-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a54a8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a54a8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a54a8-112">Permission type</span></span>                        | <span data-ttu-id="a54a8-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a54a8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a54a8-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a54a8-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="a54a8-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a54a8-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a54a8-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a54a8-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a54a8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a54a8-117">Not supported.</span></span>|
|<span data-ttu-id="a54a8-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a54a8-118">Application</span></span>                            |<span data-ttu-id="a54a8-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a54a8-119">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="a54a8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a54a8-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="a54a8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a54a8-121">Request headers</span></span>

| <span data-ttu-id="a54a8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a54a8-122">Name</span></span>           | <span data-ttu-id="a54a8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="a54a8-123">Type</span></span>    | <span data-ttu-id="a54a8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a54a8-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a54a8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a54a8-125">Authorization</span></span>  | <span data-ttu-id="a54a8-126">string</span><span class="sxs-lookup"><span data-stu-id="a54a8-126">string</span></span>  | <span data-ttu-id="a54a8-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a54a8-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a54a8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a54a8-129">Request body</span></span>

<span data-ttu-id="a54a8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a54a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a54a8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a54a8-131">Response</span></span>

<span data-ttu-id="a54a8-132">Se tiver êxito, este método retornará um código de resposta `201 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a54a8-132">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="a54a8-133">Ele não retornará nada no corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a54a8-133">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="a54a8-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a54a8-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a54a8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a54a8-135">Request</span></span>
<span data-ttu-id="a54a8-136">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a54a8-136">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="a54a8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a54a8-137">Response</span></span>
<span data-ttu-id="a54a8-138">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="a54a8-138">The following is an example of a response.</span></span>
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
