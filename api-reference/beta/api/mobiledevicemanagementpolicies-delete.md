---
title: Excluir mobileDeviceManagementPolicy
description: Exclua uma política de gerenciamento de dispositivo móvel.
author: michaelrm97
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 800cec45f578e97286982303a0e81d5b16895098
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401677"
---
# <a name="delete-mobiledevicemanagementpolicy"></a><span data-ttu-id="8de74-103">Excluir mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8de74-103">Delete mobileDeviceManagementPolicy</span></span>

<span data-ttu-id="8de74-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8de74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8de74-105">[Exclua um objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8de74-105">Delete a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="8de74-106">Essa operação só é suportada quando a política não é mais válida; ou seja, quando a **propriedade isValid** for false, o que indica que a entidade de serviço associada ao aplicativo para essa política foi excluída.</span><span class="sxs-lookup"><span data-stu-id="8de74-106">This operation is only supported when the policy is no longer valid; that is, when the **isValid** property is false, which indicates that the service principal associated with the application for this policy has been deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="8de74-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8de74-107">Permissions</span></span>

<span data-ttu-id="8de74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8de74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8de74-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8de74-110">Permission type</span></span>|<span data-ttu-id="8de74-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8de74-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8de74-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8de74-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8de74-113">Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="8de74-113">Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="8de74-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8de74-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8de74-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8de74-115">Not supported.</span></span>|
|<span data-ttu-id="8de74-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8de74-116">Application</span></span> | <span data-ttu-id="8de74-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8de74-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8de74-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8de74-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8de74-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8de74-119">Request headers</span></span>

|<span data-ttu-id="8de74-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8de74-120">Name</span></span>|<span data-ttu-id="8de74-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8de74-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8de74-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8de74-122">Authorization</span></span>|<span data-ttu-id="8de74-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8de74-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8de74-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8de74-125">Request body</span></span>

<span data-ttu-id="8de74-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8de74-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8de74-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8de74-127">Response</span></span>

<span data-ttu-id="8de74-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8de74-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8de74-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8de74-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8de74-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8de74-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_mobilitymanagementpolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```

### <a name="response"></a><span data-ttu-id="8de74-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8de74-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
