---
title: Excluir deviceInstallState
description: Exclui deviceInstallState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 60f8b7ea7da26351a2d16b21b040fe1b6fffeefe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417515"
---
# <a name="delete-deviceinstallstate"></a><span data-ttu-id="52c83-103">Excluir deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="52c83-103">Delete deviceInstallState</span></span>

> <span data-ttu-id="52c83-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="52c83-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="52c83-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="52c83-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52c83-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="52c83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52c83-107">Exclui [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="52c83-107">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52c83-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52c83-108">Prerequisites</span></span>
<span data-ttu-id="52c83-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="52c83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="52c83-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52c83-111">Permission type</span></span>|<span data-ttu-id="52c83-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52c83-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52c83-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52c83-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52c83-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52c83-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52c83-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52c83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52c83-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52c83-116">Not supported.</span></span>|
|<span data-ttu-id="52c83-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52c83-117">Application</span></span>|<span data-ttu-id="52c83-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52c83-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52c83-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52c83-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="52c83-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52c83-120">Request headers</span></span>
|<span data-ttu-id="52c83-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52c83-121">Header</span></span>|<span data-ttu-id="52c83-122">Valor</span><span class="sxs-lookup"><span data-stu-id="52c83-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52c83-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="52c83-123">Authorization</span></span>|<span data-ttu-id="52c83-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52c83-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52c83-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52c83-125">Accept</span></span>|<span data-ttu-id="52c83-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52c83-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52c83-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52c83-127">Request body</span></span>
<span data-ttu-id="52c83-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52c83-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52c83-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="52c83-129">Response</span></span>
<span data-ttu-id="52c83-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="52c83-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="52c83-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52c83-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="52c83-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52c83-132">Request</span></span>
<span data-ttu-id="52c83-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52c83-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="52c83-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="52c83-134">Response</span></span>
<span data-ttu-id="52c83-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52c83-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




