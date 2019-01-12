---
title: Excluir schemaExtension
description: Exclui uma definição da extensão de esquema.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 96b7ab5091d7e8a33bd3e94fea4a9ccc85a686fb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962797"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="1131e-103">Excluir schemaExtension</span><span class="sxs-lookup"><span data-stu-id="1131e-103">Delete schemaExtension</span></span>

> <span data-ttu-id="1131e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1131e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1131e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1131e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1131e-106">Exclui uma definição da [extensão de esquema](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="1131e-106">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="1131e-p102">Somente o aplicativo que criou a extensão de esquema (proprietário do aplicativo) pode excluir a definição da extensão de esquema e apenas quando a extensão estiver com o status **InDevelopment**. Excluir uma definição da extensão de esquema não afeta o acesso aos dados personalizados que foram adicionados às instâncias de recursos com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="1131e-p102">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="1131e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1131e-109">Permissions</span></span>
<span data-ttu-id="1131e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1131e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1131e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1131e-112">Permission type</span></span>      | <span data-ttu-id="1131e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1131e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1131e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1131e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1131e-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1131e-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1131e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1131e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1131e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1131e-117">Not supported.</span></span>    |
|<span data-ttu-id="1131e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1131e-118">Application</span></span> | <span data-ttu-id="1131e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1131e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1131e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1131e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1131e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1131e-121">Request headers</span></span>
| <span data-ttu-id="1131e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1131e-122">Name</span></span>      |<span data-ttu-id="1131e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1131e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1131e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1131e-124">Authorization</span></span>  | <span data-ttu-id="1131e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1131e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1131e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1131e-127">Request body</span></span>
<span data-ttu-id="1131e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1131e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1131e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1131e-129">Response</span></span>

<span data-ttu-id="1131e-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1131e-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1131e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1131e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1131e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1131e-133">Request</span></span>
<span data-ttu-id="1131e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1131e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="1131e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1131e-135">Response</span></span>
<span data-ttu-id="1131e-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1131e-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="1131e-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="1131e-137">See also</span></span>

- [<span data-ttu-id="1131e-138">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="1131e-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1131e-139">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="1131e-139">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
