---
title: Excluir windowsPhone81SCEPCertificateProfile
description: Exclui windowsPhone81SCEPCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76ea1371742ecd2dcaf152a929626732f6aabc5f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801285"
---
# <a name="delete-windowsphone81scepcertificateprofile"></a><span data-ttu-id="d5ff7-103">Excluir windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d5ff7-103">Delete windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="d5ff7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5ff7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5ff7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5ff7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5ff7-106">Exclui [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d5ff7-106">Deletes a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5ff7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5ff7-107">Prerequisites</span></span>
<span data-ttu-id="d5ff7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5ff7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5ff7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5ff7-110">Permission type</span></span>|<span data-ttu-id="d5ff7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5ff7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5ff7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5ff7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5ff7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5ff7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d5ff7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5ff7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5ff7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5ff7-115">Not supported.</span></span>|
|<span data-ttu-id="d5ff7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5ff7-116">Application</span></span>|<span data-ttu-id="d5ff7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5ff7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5ff7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5ff7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d5ff7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5ff7-119">Request headers</span></span>
|<span data-ttu-id="d5ff7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5ff7-120">Header</span></span>|<span data-ttu-id="d5ff7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d5ff7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5ff7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5ff7-122">Authorization</span></span>|<span data-ttu-id="d5ff7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5ff7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5ff7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5ff7-124">Accept</span></span>|<span data-ttu-id="d5ff7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5ff7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5ff7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5ff7-126">Request body</span></span>
<span data-ttu-id="d5ff7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5ff7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5ff7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5ff7-128">Response</span></span>
<span data-ttu-id="d5ff7-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d5ff7-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d5ff7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5ff7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5ff7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5ff7-131">Request</span></span>
<span data-ttu-id="d5ff7-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5ff7-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d5ff7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5ff7-133">Response</span></span>
<span data-ttu-id="d5ff7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5ff7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





