---
title: Excluir synchronizationSchema
description: Exclui o esquema personalizado e redefine o esquema para a configuração padrão. Se o esquema for excluído no contexto do modelo, ele redefinirá o esquema como o padrão associado ao modelo do `factoryTag`.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: de8e8eaf2d8a5473a530c8497aca7e40739ed19c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443354"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="f852e-104">Excluir synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="f852e-104">Delete synchronizationSchema</span></span>

<span data-ttu-id="f852e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f852e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f852e-106">Exclui o esquema personalizado e redefine o esquema para a configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="f852e-106">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="f852e-107">Se o esquema for excluído no contexto do modelo, ele redefinirá o esquema como o padrão associado ao modelo do `factoryTag`.</span><span class="sxs-lookup"><span data-stu-id="f852e-107">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="f852e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f852e-108">Permissions</span></span>
<span data-ttu-id="f852e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f852e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f852e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f852e-111">Permission type</span></span>                        | <span data-ttu-id="f852e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f852e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f852e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f852e-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="f852e-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f852e-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f852e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f852e-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f852e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f852e-116">Not supported.</span></span>|
|<span data-ttu-id="f852e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f852e-117">Application</span></span>                            |<span data-ttu-id="f852e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f852e-118">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="f852e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f852e-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="f852e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f852e-120">Request headers</span></span>

| <span data-ttu-id="f852e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f852e-121">Name</span></span>           | <span data-ttu-id="f852e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f852e-122">Type</span></span>    | <span data-ttu-id="f852e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f852e-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f852e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f852e-124">Authorization</span></span>  | <span data-ttu-id="f852e-125">string</span><span class="sxs-lookup"><span data-stu-id="f852e-125">string</span></span>  | <span data-ttu-id="f852e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f852e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f852e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f852e-128">Request body</span></span>

<span data-ttu-id="f852e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f852e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f852e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f852e-130">Response</span></span>

<span data-ttu-id="f852e-131">Se tiver êxito, este método retornará um código de resposta `201 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f852e-131">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="f852e-132">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f852e-132">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="f852e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f852e-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f852e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f852e-134">Request</span></span>
<span data-ttu-id="f852e-135">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f852e-135">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="f852e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f852e-136">Response</span></span>
<span data-ttu-id="f852e-137">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f852e-137">The following is an example of a response.</span></span>
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
