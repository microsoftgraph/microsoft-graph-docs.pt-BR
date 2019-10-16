---
title: Excluir mobileAppIntentAndState
description: Exclui mobileAppIntentAndState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de897da4bee7976130d19acc1c9325c894a11e5a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536711"
---
# <a name="delete-mobileappintentandstate"></a><span data-ttu-id="88c99-103">Excluir mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="88c99-103">Delete mobileAppIntentAndState</span></span>

> <span data-ttu-id="88c99-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88c99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88c99-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88c99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88c99-106">Exclui [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span><span class="sxs-lookup"><span data-stu-id="88c99-106">Deletes a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88c99-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88c99-107">Prerequisites</span></span>
<span data-ttu-id="88c99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88c99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88c99-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88c99-110">Permission type</span></span>|<span data-ttu-id="88c99-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88c99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88c99-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88c99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88c99-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c99-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="88c99-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88c99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88c99-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88c99-115">Not supported.</span></span>|
|<span data-ttu-id="88c99-116">Application</span><span class="sxs-lookup"><span data-stu-id="88c99-116">Application</span></span>|<span data-ttu-id="88c99-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c99-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88c99-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88c99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="88c99-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88c99-119">Request headers</span></span>
|<span data-ttu-id="88c99-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88c99-120">Header</span></span>|<span data-ttu-id="88c99-121">Valor</span><span class="sxs-lookup"><span data-stu-id="88c99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88c99-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="88c99-122">Authorization</span></span>|<span data-ttu-id="88c99-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88c99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88c99-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88c99-124">Accept</span></span>|<span data-ttu-id="88c99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88c99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88c99-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88c99-126">Request body</span></span>
<span data-ttu-id="88c99-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88c99-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88c99-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="88c99-128">Response</span></span>
<span data-ttu-id="88c99-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="88c99-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="88c99-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88c99-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="88c99-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88c99-131">Request</span></span>
<span data-ttu-id="88c99-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88c99-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### <a name="response"></a><span data-ttu-id="88c99-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="88c99-133">Response</span></span>
<span data-ttu-id="88c99-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88c99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






