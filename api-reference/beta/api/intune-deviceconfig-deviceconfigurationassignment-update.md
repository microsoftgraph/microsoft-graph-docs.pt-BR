---
title: Atualizar deviceConfigurationAssignment
description: Atualizar as propriedades de um objeto deviceConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f15174d943d880e805a96f148e1665dcaffa504e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967864"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="abf22-103">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="abf22-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="abf22-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abf22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abf22-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abf22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abf22-106">Atualizar as propriedades de um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abf22-106">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abf22-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abf22-107">Prerequisites</span></span>
<span data-ttu-id="abf22-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abf22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abf22-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abf22-110">Permission type</span></span>|<span data-ttu-id="abf22-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abf22-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abf22-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abf22-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abf22-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abf22-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abf22-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abf22-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abf22-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abf22-115">Not supported.</span></span>|
|<span data-ttu-id="abf22-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abf22-116">Application</span></span>|<span data-ttu-id="abf22-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abf22-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abf22-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abf22-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="abf22-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abf22-119">Request headers</span></span>
|<span data-ttu-id="abf22-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abf22-120">Header</span></span>|<span data-ttu-id="abf22-121">Valor</span><span class="sxs-lookup"><span data-stu-id="abf22-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abf22-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="abf22-122">Authorization</span></span>|<span data-ttu-id="abf22-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abf22-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abf22-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abf22-124">Accept</span></span>|<span data-ttu-id="abf22-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abf22-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abf22-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abf22-126">Request body</span></span>
<span data-ttu-id="abf22-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abf22-127">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="abf22-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abf22-128">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="abf22-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abf22-129">Property</span></span>|<span data-ttu-id="abf22-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="abf22-130">Type</span></span>|<span data-ttu-id="abf22-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="abf22-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abf22-132">id</span><span class="sxs-lookup"><span data-stu-id="abf22-132">id</span></span>|<span data-ttu-id="abf22-133">String</span><span class="sxs-lookup"><span data-stu-id="abf22-133">String</span></span>|<span data-ttu-id="abf22-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="abf22-134">The key of the assignment.</span></span>|
|<span data-ttu-id="abf22-135">destino</span><span class="sxs-lookup"><span data-stu-id="abf22-135">target</span></span>|[<span data-ttu-id="abf22-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="abf22-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="abf22-137">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="abf22-137">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="abf22-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="abf22-138">Response</span></span>
<span data-ttu-id="abf22-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abf22-139">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abf22-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abf22-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="abf22-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abf22-141">Request</span></span>
<span data-ttu-id="abf22-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abf22-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="abf22-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="abf22-143">Response</span></span>
<span data-ttu-id="abf22-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abf22-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





