---
title: Listar identityUserFlowAttributes
description: Recupere uma lista de objetos identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c5a6aa380f1f8dfea25de5d15fb29e04ec3e0e9c
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742344"
---
# <a name="list-identityuserflowattributes"></a><span data-ttu-id="52b54-103">Listar identityUserFlowAttributes</span><span class="sxs-lookup"><span data-stu-id="52b54-103">List identityUserFlowAttributes</span></span>

<span data-ttu-id="52b54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52b54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52b54-105">Recupere uma lista de objetos [identityUserFlowAttribute](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="52b54-105">Retrieve a list of [identityUserFlowAttribute](../resources/identityuserflowattribute.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="52b54-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="52b54-106">Permissions</span></span>

<span data-ttu-id="52b54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52b54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52b54-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52b54-109">Permission type</span></span>      | <span data-ttu-id="52b54-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52b54-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52b54-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52b54-111">Delegated (work or school account)</span></span>|<span data-ttu-id="52b54-112">IdentityUserFlow. Read. All, IdentityUserflow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="52b54-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span></span>|
|<span data-ttu-id="52b54-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52b54-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="52b54-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52b54-114">Not supported.</span></span>|
|<span data-ttu-id="52b54-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52b54-115">Application</span></span>|<span data-ttu-id="52b54-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="52b54-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="52b54-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="52b54-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="52b54-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="52b54-118">Global administrator</span></span>
* <span data-ttu-id="52b54-119">Administrador do atributo de fluxo do usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="52b54-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="52b54-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52b54-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="52b54-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52b54-121">Request headers</span></span>

|<span data-ttu-id="52b54-122">Nome</span><span class="sxs-lookup"><span data-stu-id="52b54-122">Name</span></span>|<span data-ttu-id="52b54-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="52b54-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="52b54-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="52b54-124">Authorization</span></span>|<span data-ttu-id="52b54-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52b54-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52b54-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52b54-127">Request body</span></span>

<span data-ttu-id="52b54-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52b54-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52b54-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="52b54-129">Response</span></span>

<span data-ttu-id="52b54-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52b54-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52b54-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52b54-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="52b54-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52b54-132">Request</span></span>

<span data-ttu-id="52b54-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52b54-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes
```

### <a name="response"></a><span data-ttu-id="52b54-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="52b54-134">Response</span></span>

<span data-ttu-id="52b54-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52b54-135">The following is an example of the response.</span></span>

<span data-ttu-id="52b54-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52b54-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#userFlowAttributes",
    "value": [
      {
          "id": "City",
          "displayName": "City",
          "description": "Your city",
          "userFlowAttributeType": "builtIn",
          "dataType": "string"
      },
      {
          "id": "extension_d09380e2b4c6429a203fb816a04a7ad_Hobby",
          "displayName": "Hobby",
          "description": "Your hobby",
          "userFlowAttributeType": "custom",
          "dataType": "string",
      },
    ]
}
```
