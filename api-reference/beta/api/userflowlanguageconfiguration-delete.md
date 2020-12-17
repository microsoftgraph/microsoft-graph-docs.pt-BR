---
title: Excluir userFlowLanguageConfiguration
description: Exclui um objeto userFlowLanguageConfiguration de um fluxo de usuário do B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f9396e9522e4f2f6df536e687526b261ce78e6b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706251"
---
# <a name="delete-userflowlanguageconfiguration"></a><span data-ttu-id="c96f8-103">Excluir userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="c96f8-103">Delete userFlowLanguageConfiguration</span></span>

<span data-ttu-id="c96f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c96f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c96f8-105">Exclui um objeto [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) de um [fluxo de usuário do Azure ad B2C](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="c96f8-105">Deletes a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object from a [Azure AD B2C user flow](../resources/b2cidentityuserflow.md).</span></span>

<span data-ttu-id="c96f8-106">**Observação:** Não é possível excluir idiomas de um [fluxo de usuário do Azure Active Directory](../resources/b2xidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="c96f8-106">**Note:** You cannot delete languages from an [Azure Active Directory user flow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c96f8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c96f8-107">Permissions</span></span>

<span data-ttu-id="c96f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c96f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c96f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c96f8-110">Permission type</span></span>      | <span data-ttu-id="c96f8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c96f8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c96f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c96f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c96f8-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c96f8-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c96f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c96f8-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c96f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c96f8-115">Not supported.</span></span>|
|<span data-ttu-id="c96f8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c96f8-116">Application</span></span>|<span data-ttu-id="c96f8-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c96f8-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c96f8-118">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c96f8-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c96f8-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c96f8-119">Global administrator</span></span>
* <span data-ttu-id="c96f8-120">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="c96f8-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c96f8-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c96f8-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c96f8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c96f8-122">Request headers</span></span>

|<span data-ttu-id="c96f8-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c96f8-123">Name</span></span>|<span data-ttu-id="c96f8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c96f8-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c96f8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c96f8-125">Authorization</span></span>|<span data-ttu-id="c96f8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c96f8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c96f8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c96f8-128">Request body</span></span>

<span data-ttu-id="c96f8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c96f8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c96f8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c96f8-130">Response</span></span>

<span data-ttu-id="c96f8-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c96f8-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c96f8-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c96f8-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c96f8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c96f8-133">Request</span></span>

<span data-ttu-id="c96f8-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c96f8-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguageconfiguration"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/es-ES
```

### <a name="response"></a><span data-ttu-id="c96f8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c96f8-135">Response</span></span>

<span data-ttu-id="c96f8-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c96f8-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
