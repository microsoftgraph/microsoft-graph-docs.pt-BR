---
title: Criar synchronizationTemplate
description: Crie um novo modelo de sincronização para um determinado aplicativo.
localization_priority: Normal
ms.openlocfilehash: 5b52c2ef180781faf8c93ce335d5f22ca8ae57cd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822698"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="c19eb-103">Criar synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="c19eb-103">Create synchronizationTemplate</span></span>

> <span data-ttu-id="c19eb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c19eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c19eb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c19eb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c19eb-106">Crie um novo modelo de sincronização para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c19eb-106">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="c19eb-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="c19eb-107">Permissions</span></span>
<span data-ttu-id="c19eb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c19eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c19eb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c19eb-110">Permission type</span></span>                        | <span data-ttu-id="c19eb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c19eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c19eb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c19eb-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="c19eb-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c19eb-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c19eb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c19eb-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c19eb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c19eb-115">Not supported.</span></span>|
|<span data-ttu-id="c19eb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c19eb-116">Application</span></span>                            |<span data-ttu-id="c19eb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c19eb-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="c19eb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c19eb-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="c19eb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c19eb-119">Request headers</span></span>

| <span data-ttu-id="c19eb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c19eb-120">Name</span></span>           | <span data-ttu-id="c19eb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c19eb-121">Type</span></span>    | <span data-ttu-id="c19eb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c19eb-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c19eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c19eb-123">Authorization</span></span>  | <span data-ttu-id="c19eb-124">string</span><span class="sxs-lookup"><span data-stu-id="c19eb-124">string</span></span>  | <span data-ttu-id="c19eb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c19eb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c19eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c19eb-127">Request body</span></span>

<span data-ttu-id="c19eb-128">No corpo da solicitação, fornece o objeto [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) a ser criado.</span><span class="sxs-lookup"><span data-stu-id="c19eb-128">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="c19eb-129">O `id`, `applicationId` e `factoryTag` propriedades são necessárias.</span><span class="sxs-lookup"><span data-stu-id="c19eb-129">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="c19eb-130">Quando não `schema` é fornecida com o modelo, o esquema padrão associado a `factoryTag` propriedade será usada.</span><span class="sxs-lookup"><span data-stu-id="c19eb-130">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="c19eb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c19eb-131">Response</span></span>

<span data-ttu-id="c19eb-132">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c19eb-132">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="c19eb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c19eb-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c19eb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c19eb-134">Request</span></span>
<span data-ttu-id="c19eb-135">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c19eb-135">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/synchronization/templates
Content-type: application/json

{ 
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="c19eb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c19eb-136">Response</span></span>
<span data-ttu-id="c19eb-137">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c19eb-137">The following is an example of a response.</span></span>
><span data-ttu-id="c19eb-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c19eb-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c19eb-139">Serão retornadas todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c19eb-139">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created

{
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
