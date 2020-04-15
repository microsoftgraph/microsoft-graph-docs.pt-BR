---
title: Excluir androidGeneralDeviceConfiguration
description: Exclui androidGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 62b87f0d3462708be78b8a52cbdd59c06d3d5f52
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474646"
---
# <a name="delete-androidgeneraldeviceconfiguration"></a><span data-ttu-id="4fe88-103">Excluir androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4fe88-103">Delete androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="4fe88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fe88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fe88-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4fe88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fe88-106">Exclui [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fe88-106">Deletes a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fe88-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4fe88-107">Prerequisites</span></span>
<span data-ttu-id="4fe88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fe88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fe88-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fe88-110">Permission type</span></span>|<span data-ttu-id="4fe88-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4fe88-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fe88-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fe88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fe88-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fe88-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4fe88-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fe88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fe88-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fe88-115">Not supported.</span></span>|
|<span data-ttu-id="4fe88-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4fe88-116">Application</span></span>|<span data-ttu-id="4fe88-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fe88-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fe88-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fe88-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4fe88-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fe88-119">Request headers</span></span>
|<span data-ttu-id="4fe88-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4fe88-120">Header</span></span>|<span data-ttu-id="4fe88-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4fe88-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fe88-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fe88-122">Authorization</span></span>|<span data-ttu-id="4fe88-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fe88-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fe88-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4fe88-124">Accept</span></span>|<span data-ttu-id="4fe88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4fe88-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fe88-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4fe88-126">Request body</span></span>
<span data-ttu-id="4fe88-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4fe88-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fe88-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fe88-128">Response</span></span>
<span data-ttu-id="4fe88-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4fe88-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4fe88-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fe88-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fe88-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fe88-131">Request</span></span>
<span data-ttu-id="4fe88-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fe88-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4fe88-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fe88-133">Response</span></span>
<span data-ttu-id="4fe88-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4fe88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






