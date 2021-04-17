---
title: Obter userFlowLanguageConfiguration
description: Leia as propriedades e as relações de um objeto userFlowLanguageConfiguration.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 054ed16948c86b872ee82572c770425e1c7b457b
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882754"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="7477d-103">Obter userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="7477d-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="7477d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7477d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7477d-105">Leia as propriedades e as relações de um [objeto userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7477d-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="7477d-106">Esses objetos representam um idioma disponível em um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="7477d-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="7477d-107">**Observação:** A personalização de idioma é habilitada por padrão nos fluxos de [usuários do Azure Active Directory.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="7477d-107">**Note:** Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7477d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7477d-108">Permissions</span></span>

<span data-ttu-id="7477d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7477d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7477d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7477d-111">Permission type</span></span>      | <span data-ttu-id="7477d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7477d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7477d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7477d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7477d-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7477d-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="7477d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7477d-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7477d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7477d-116">Not supported.</span></span>|
|<span data-ttu-id="7477d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7477d-117">Application</span></span>|<span data-ttu-id="7477d-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7477d-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="7477d-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="7477d-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7477d-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7477d-120">Global administrator</span></span>
* <span data-ttu-id="7477d-121">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="7477d-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7477d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7477d-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7477d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7477d-123">Request headers</span></span>

|<span data-ttu-id="7477d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7477d-124">Name</span></span>|<span data-ttu-id="7477d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7477d-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7477d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7477d-126">Authorization</span></span>|<span data-ttu-id="7477d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7477d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7477d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7477d-129">Request body</span></span>

<span data-ttu-id="7477d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7477d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7477d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7477d-131">Response</span></span>

<span data-ttu-id="7477d-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7477d-132">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7477d-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7477d-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7477d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7477d-134">Request</span></span>

<span data-ttu-id="7477d-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7477d-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en
```

### <a name="response"></a><span data-ttu-id="7477d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7477d-136">Response</span></span>

<span data-ttu-id="7477d-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7477d-137">The following is an example of the response.</span></span>

<span data-ttu-id="7477d-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7477d-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_Partner')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
