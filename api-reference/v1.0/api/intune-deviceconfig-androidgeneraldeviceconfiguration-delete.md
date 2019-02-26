---
title: Excluir androidGeneralDeviceConfiguration
description: Exclui androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 047ea3855fc3e4cd2ca639adf04472ad36d19a24
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254258"
---
# <a name="delete-androidgeneraldeviceconfiguration"></a><span data-ttu-id="b5aae-103">Excluir androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5aae-103">Delete androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="b5aae-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5aae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5aae-105">Exclui [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5aae-105">Deletes a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5aae-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b5aae-106">Prerequisites</span></span>
<span data-ttu-id="b5aae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5aae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b5aae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5aae-109">Permission type</span></span>|<span data-ttu-id="b5aae-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b5aae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5aae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5aae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b5aae-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5aae-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5aae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5aae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5aae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5aae-114">Not supported.</span></span>|
|<span data-ttu-id="b5aae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5aae-115">Application</span></span>|<span data-ttu-id="b5aae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5aae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5aae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5aae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b5aae-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5aae-118">Request headers</span></span>
|<span data-ttu-id="b5aae-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5aae-119">Header</span></span>|<span data-ttu-id="b5aae-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b5aae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5aae-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5aae-121">Authorization</span></span>|<span data-ttu-id="b5aae-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5aae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5aae-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b5aae-123">Accept</span></span>|<span data-ttu-id="b5aae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b5aae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5aae-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5aae-125">Request body</span></span>
<span data-ttu-id="b5aae-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5aae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5aae-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5aae-127">Response</span></span>
<span data-ttu-id="b5aae-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b5aae-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b5aae-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5aae-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5aae-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5aae-130">Request</span></span>
<span data-ttu-id="b5aae-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5aae-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b5aae-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5aae-132">Response</span></span>
<span data-ttu-id="b5aae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5aae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



