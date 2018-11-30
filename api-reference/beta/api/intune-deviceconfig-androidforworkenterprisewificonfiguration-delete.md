---
title: Excluir androidForWorkEnterpriseWiFiConfiguration
description: Exclui um androidForWorkEnterpriseWiFiConfiguration.
ms.openlocfilehash: 8d16f89dc8340f56b258b50eb7c1ff77c74651cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037614"
---
# <a name="delete-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="42597-103">Excluir androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="42597-103">Delete androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="42597-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="42597-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42597-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="42597-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42597-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="42597-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42597-107">Exclui um [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42597-107">Deletes a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="42597-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42597-108">Prerequisites</span></span>
<span data-ttu-id="42597-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42597-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42597-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42597-111">Permission type</span></span>|<span data-ttu-id="42597-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42597-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42597-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42597-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42597-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42597-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42597-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42597-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42597-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42597-116">Not supported.</span></span>|
|<span data-ttu-id="42597-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42597-117">Application</span></span>|<span data-ttu-id="42597-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42597-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42597-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42597-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="42597-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42597-120">Request headers</span></span>
|<span data-ttu-id="42597-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42597-121">Header</span></span>|<span data-ttu-id="42597-122">Valor</span><span class="sxs-lookup"><span data-stu-id="42597-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42597-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42597-123">Authorization</span></span>|<span data-ttu-id="42597-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42597-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42597-125">Accept</span><span class="sxs-lookup"><span data-stu-id="42597-125">Accept</span></span>|<span data-ttu-id="42597-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42597-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42597-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42597-127">Request body</span></span>
<span data-ttu-id="42597-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42597-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42597-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="42597-129">Response</span></span>
<span data-ttu-id="42597-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="42597-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="42597-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42597-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="42597-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42597-132">Request</span></span>
<span data-ttu-id="42597-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42597-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="42597-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="42597-134">Response</span></span>
<span data-ttu-id="42597-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42597-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





