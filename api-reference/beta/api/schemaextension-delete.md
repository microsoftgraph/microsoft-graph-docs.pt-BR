---
title: Excluir schemaExtension
description: Exclui uma definição da extensão de esquema.
localization_priority: Normal
ms.openlocfilehash: 8641b00b984380592f14ae366b9cc20ab11dc7b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842193"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="84316-103">Excluir schemaExtension</span><span class="sxs-lookup"><span data-stu-id="84316-103">Delete schemaExtension</span></span>

> <span data-ttu-id="84316-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="84316-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84316-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="84316-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="84316-106">Exclui uma definição da [extensão de esquema](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="84316-106">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="84316-p102">Somente o aplicativo que criou a extensão de esquema (proprietário do aplicativo) pode excluir a definição da extensão de esquema e apenas quando a extensão estiver com o status **InDevelopment**. Excluir uma definição da extensão de esquema não afeta o acesso aos dados personalizados que foram adicionados às instâncias de recursos com base nessa definição.</span><span class="sxs-lookup"><span data-stu-id="84316-p102">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="84316-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="84316-109">Permissions</span></span>
<span data-ttu-id="84316-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84316-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="84316-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84316-112">Permission type</span></span>      | <span data-ttu-id="84316-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84316-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84316-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84316-114">Delegated (work or school account)</span></span> | <span data-ttu-id="84316-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="84316-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="84316-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84316-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84316-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84316-117">Not supported.</span></span>    |
|<span data-ttu-id="84316-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84316-118">Application</span></span> | <span data-ttu-id="84316-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84316-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84316-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84316-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="84316-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84316-121">Request headers</span></span>
| <span data-ttu-id="84316-122">Nome</span><span class="sxs-lookup"><span data-stu-id="84316-122">Name</span></span>      |<span data-ttu-id="84316-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="84316-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84316-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="84316-124">Authorization</span></span>  | <span data-ttu-id="84316-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84316-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84316-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84316-127">Request body</span></span>
<span data-ttu-id="84316-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84316-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84316-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="84316-129">Response</span></span>

<span data-ttu-id="84316-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84316-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84316-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84316-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84316-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84316-133">Request</span></span>
<span data-ttu-id="84316-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84316-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="84316-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="84316-135">Response</span></span>
<span data-ttu-id="84316-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84316-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="84316-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="84316-137">See also</span></span>

- [<span data-ttu-id="84316-138">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="84316-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="84316-139">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="84316-139">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
