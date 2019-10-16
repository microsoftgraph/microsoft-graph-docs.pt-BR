---
title: Excluir iosLobAppProvisioningConfiguration
description: Exclui iosLobAppProvisioningConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1da9289daaf5b66f4eae6b6a6c1b79ad8689d86a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538347"
---
# <a name="delete-ioslobappprovisioningconfiguration"></a><span data-ttu-id="e6020-103">Excluir iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="e6020-103">Delete iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="e6020-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6020-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6020-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6020-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6020-106">Exclui [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6020-106">Deletes a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6020-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6020-107">Prerequisites</span></span>
<span data-ttu-id="e6020-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6020-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6020-110">Permission type</span></span>|<span data-ttu-id="e6020-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6020-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6020-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6020-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e6020-113">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="e6020-113">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="e6020-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6020-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="e6020-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="e6020-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e6020-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6020-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e6020-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6020-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6020-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6020-118">Not supported.</span></span>|
|<span data-ttu-id="e6020-119">Application</span><span class="sxs-lookup"><span data-stu-id="e6020-119">Application</span></span>||
| <span data-ttu-id="e6020-120">&nbsp;&nbsp; **Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="e6020-120">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="e6020-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6020-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="e6020-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="e6020-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e6020-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6020-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6020-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6020-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e6020-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6020-125">Request headers</span></span>
|<span data-ttu-id="e6020-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6020-126">Header</span></span>|<span data-ttu-id="e6020-127">Valor</span><span class="sxs-lookup"><span data-stu-id="e6020-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6020-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6020-128">Authorization</span></span>|<span data-ttu-id="e6020-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6020-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6020-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6020-130">Accept</span></span>|<span data-ttu-id="e6020-131">application/json</span><span class="sxs-lookup"><span data-stu-id="e6020-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6020-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6020-132">Request body</span></span>
<span data-ttu-id="e6020-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6020-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6020-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6020-134">Response</span></span>
<span data-ttu-id="e6020-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6020-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e6020-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6020-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6020-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6020-137">Request</span></span>
<span data-ttu-id="e6020-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6020-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e6020-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6020-139">Response</span></span>
<span data-ttu-id="e6020-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6020-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






