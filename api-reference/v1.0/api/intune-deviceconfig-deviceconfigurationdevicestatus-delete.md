---
title: Excluir deviceConfigurationDeviceStatus
description: Exclui deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5597e4134b00e6b9745af907bd8d573e0ea1a106
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460526"
---
# <a name="delete-deviceconfigurationdevicestatus"></a><span data-ttu-id="af2f2-103">Excluir deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="af2f2-103">Delete deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="af2f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af2f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af2f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af2f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af2f2-106">Exclui [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="af2f2-106">Deletes a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af2f2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="af2f2-107">Prerequisites</span></span>
<span data-ttu-id="af2f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af2f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af2f2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af2f2-110">Permission type</span></span>|<span data-ttu-id="af2f2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="af2f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af2f2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af2f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af2f2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af2f2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af2f2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af2f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af2f2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af2f2-115">Not supported.</span></span>|
|<span data-ttu-id="af2f2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af2f2-116">Application</span></span>|<span data-ttu-id="af2f2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af2f2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af2f2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af2f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="af2f2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af2f2-119">Request headers</span></span>
|<span data-ttu-id="af2f2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af2f2-120">Header</span></span>|<span data-ttu-id="af2f2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="af2f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af2f2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="af2f2-122">Authorization</span></span>|<span data-ttu-id="af2f2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af2f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af2f2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="af2f2-124">Accept</span></span>|<span data-ttu-id="af2f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af2f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af2f2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af2f2-126">Request body</span></span>
<span data-ttu-id="af2f2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af2f2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af2f2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="af2f2-128">Response</span></span>
<span data-ttu-id="af2f2-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="af2f2-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="af2f2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af2f2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="af2f2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af2f2-131">Request</span></span>
<span data-ttu-id="af2f2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af2f2-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="af2f2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="af2f2-133">Response</span></span>
<span data-ttu-id="af2f2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af2f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






