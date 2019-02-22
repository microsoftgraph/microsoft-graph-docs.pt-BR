---
title: Excluir androidImportedPFXCertificateProfile
description: Exclui androidImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32e0440e7e87aae575fc9b0876658521d32f41df
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153078"
---
# <a name="delete-androidimportedpfxcertificateprofile"></a><span data-ttu-id="3994f-103">Excluir androidImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="3994f-103">Delete androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="3994f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3994f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3994f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3994f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3994f-106">Exclui [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="3994f-106">Deletes a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3994f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3994f-107">Prerequisites</span></span>
<span data-ttu-id="3994f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3994f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3994f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3994f-110">Permission type</span></span>|<span data-ttu-id="3994f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3994f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3994f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3994f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3994f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3994f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3994f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3994f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3994f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3994f-115">Not supported.</span></span>|
|<span data-ttu-id="3994f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3994f-116">Application</span></span>|<span data-ttu-id="3994f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3994f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3994f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3994f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3994f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3994f-119">Request headers</span></span>
|<span data-ttu-id="3994f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3994f-120">Header</span></span>|<span data-ttu-id="3994f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3994f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3994f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3994f-122">Authorization</span></span>|<span data-ttu-id="3994f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3994f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3994f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3994f-124">Accept</span></span>|<span data-ttu-id="3994f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3994f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3994f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3994f-126">Request body</span></span>
<span data-ttu-id="3994f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3994f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3994f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3994f-128">Response</span></span>
<span data-ttu-id="3994f-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3994f-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3994f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3994f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3994f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3994f-131">Request</span></span>
<span data-ttu-id="3994f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3994f-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3994f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3994f-133">Response</span></span>
<span data-ttu-id="3994f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3994f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




