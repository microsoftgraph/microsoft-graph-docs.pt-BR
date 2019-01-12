---
title: Excluir macOSWiFiConfiguration
description: Exclui um macOSWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3083dfe38cc26d51a4e3be85d41c6e82f6924aa4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945451"
---
# <a name="delete-macoswificonfiguration"></a><span data-ttu-id="afdad-103">Excluir macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="afdad-103">Delete macOSWiFiConfiguration</span></span>

> <span data-ttu-id="afdad-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="afdad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afdad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="afdad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="afdad-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="afdad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afdad-107">Exclui um [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="afdad-107">Deletes a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="afdad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="afdad-108">Prerequisites</span></span>
<span data-ttu-id="afdad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afdad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afdad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afdad-111">Permission type</span></span>|<span data-ttu-id="afdad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="afdad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afdad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afdad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afdad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afdad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="afdad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afdad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afdad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afdad-116">Not supported.</span></span>|
|<span data-ttu-id="afdad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afdad-117">Application</span></span>|<span data-ttu-id="afdad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afdad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afdad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afdad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="afdad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afdad-120">Request headers</span></span>
|<span data-ttu-id="afdad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="afdad-121">Header</span></span>|<span data-ttu-id="afdad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="afdad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afdad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="afdad-123">Authorization</span></span>|<span data-ttu-id="afdad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afdad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afdad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="afdad-125">Accept</span></span>|<span data-ttu-id="afdad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afdad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afdad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afdad-127">Request body</span></span>
<span data-ttu-id="afdad-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="afdad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afdad-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="afdad-129">Response</span></span>
<span data-ttu-id="afdad-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="afdad-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="afdad-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afdad-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="afdad-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afdad-132">Request</span></span>
<span data-ttu-id="afdad-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="afdad-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="afdad-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="afdad-134">Response</span></span>
<span data-ttu-id="afdad-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afdad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





