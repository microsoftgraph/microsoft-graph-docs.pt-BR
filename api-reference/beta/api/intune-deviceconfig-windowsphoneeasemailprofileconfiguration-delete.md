---
title: Excluir windowsPhoneEASEmailProfileConfiguration
description: Exclui windowsPhoneEASEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc521b9f2a95312034e23b0ef72389c2079b1a5a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972326"
---
# <a name="delete-windowsphoneeasemailprofileconfiguration"></a><span data-ttu-id="22058-103">Excluir windowsPhoneEASEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="22058-103">Delete windowsPhoneEASEmailProfileConfiguration</span></span>

<span data-ttu-id="22058-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22058-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22058-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22058-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22058-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22058-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22058-107">Exclui [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22058-107">Deletes a [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22058-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22058-108">Prerequisites</span></span>
<span data-ttu-id="22058-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22058-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22058-111">Permission type</span></span>|<span data-ttu-id="22058-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22058-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22058-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22058-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22058-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22058-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22058-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22058-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22058-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22058-116">Not supported.</span></span>|
|<span data-ttu-id="22058-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22058-117">Application</span></span>|<span data-ttu-id="22058-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22058-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22058-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22058-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="22058-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22058-120">Request headers</span></span>
|<span data-ttu-id="22058-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22058-121">Header</span></span>|<span data-ttu-id="22058-122">Valor</span><span class="sxs-lookup"><span data-stu-id="22058-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22058-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22058-123">Authorization</span></span>|<span data-ttu-id="22058-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22058-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22058-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22058-125">Accept</span></span>|<span data-ttu-id="22058-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22058-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22058-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22058-127">Request body</span></span>
<span data-ttu-id="22058-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22058-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22058-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="22058-129">Response</span></span>
<span data-ttu-id="22058-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="22058-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="22058-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22058-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="22058-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22058-132">Request</span></span>
<span data-ttu-id="22058-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22058-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="22058-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="22058-134">Response</span></span>
<span data-ttu-id="22058-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22058-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






