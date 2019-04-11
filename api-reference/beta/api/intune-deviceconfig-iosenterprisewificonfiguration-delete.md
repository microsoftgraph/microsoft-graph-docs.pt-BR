---
title: Excluir iosEnterpriseWiFiConfiguration
description: Exclui iosEnterpriseWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38796bcd7e379cae0ddac5ec17f00a290c3091f1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788860"
---
# <a name="delete-iosenterprisewificonfiguration"></a><span data-ttu-id="79223-103">Excluir iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="79223-103">Delete iosEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="79223-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79223-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79223-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79223-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79223-106">Exclui [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79223-106">Deletes a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79223-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79223-107">Prerequisites</span></span>
<span data-ttu-id="79223-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79223-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79223-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79223-110">Permission type</span></span>|<span data-ttu-id="79223-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79223-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79223-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79223-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79223-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79223-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79223-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79223-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79223-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79223-115">Not supported.</span></span>|
|<span data-ttu-id="79223-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79223-116">Application</span></span>|<span data-ttu-id="79223-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79223-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79223-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79223-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="79223-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79223-119">Request headers</span></span>
|<span data-ttu-id="79223-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79223-120">Header</span></span>|<span data-ttu-id="79223-121">Valor</span><span class="sxs-lookup"><span data-stu-id="79223-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79223-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="79223-122">Authorization</span></span>|<span data-ttu-id="79223-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79223-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79223-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79223-124">Accept</span></span>|<span data-ttu-id="79223-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79223-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79223-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79223-126">Request body</span></span>
<span data-ttu-id="79223-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79223-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79223-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="79223-128">Response</span></span>
<span data-ttu-id="79223-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="79223-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="79223-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79223-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="79223-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79223-131">Request</span></span>
<span data-ttu-id="79223-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79223-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="79223-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="79223-133">Response</span></span>
<span data-ttu-id="79223-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79223-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





