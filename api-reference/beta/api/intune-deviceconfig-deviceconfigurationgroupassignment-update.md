---
title: Atualizar deviceConfigurationGroupAssignment
description: Atualiza as propriedades de um objeto deviceConfigurationGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8471c894bc7c879fc8657367640163db4ad9e52b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449135"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="c0117-103">Atualizar deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="c0117-103">Update deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="c0117-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c0117-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0117-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0117-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0117-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0117-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0117-107">Atualiza as propriedades de um objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c0117-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0117-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0117-108">Prerequisites</span></span>
<span data-ttu-id="c0117-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0117-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0117-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0117-111">Permission type</span></span>|<span data-ttu-id="c0117-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0117-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0117-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0117-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0117-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0117-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0117-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0117-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0117-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0117-116">Not supported.</span></span>|
|<span data-ttu-id="c0117-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0117-117">Application</span></span>|<span data-ttu-id="c0117-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0117-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0117-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0117-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c0117-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0117-120">Request headers</span></span>
|<span data-ttu-id="c0117-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0117-121">Header</span></span>|<span data-ttu-id="c0117-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c0117-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0117-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0117-123">Authorization</span></span>|<span data-ttu-id="c0117-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0117-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0117-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0117-125">Accept</span></span>|<span data-ttu-id="c0117-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0117-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0117-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0117-127">Request body</span></span>
<span data-ttu-id="c0117-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c0117-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="c0117-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0117-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="c0117-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0117-130">Property</span></span>|<span data-ttu-id="c0117-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0117-131">Type</span></span>|<span data-ttu-id="c0117-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0117-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0117-133">id</span><span class="sxs-lookup"><span data-stu-id="c0117-133">id</span></span>|<span data-ttu-id="c0117-134">String</span><span class="sxs-lookup"><span data-stu-id="c0117-134">String</span></span>|<span data-ttu-id="c0117-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c0117-135">Key of the entity.</span></span>|
|<span data-ttu-id="c0117-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="c0117-136">targetGroupId</span></span>|<span data-ttu-id="c0117-137">String</span><span class="sxs-lookup"><span data-stu-id="c0117-137">String</span></span>|<span data-ttu-id="c0117-138">A ID do grupo do AAD no qual estamos direcionando a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0117-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="c0117-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="c0117-139">excludeGroup</span></span>|<span data-ttu-id="c0117-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0117-140">Boolean</span></span>|<span data-ttu-id="c0117-141">Indica se esse grupo deve ser excluído.</span><span class="sxs-lookup"><span data-stu-id="c0117-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="c0117-142">Padrões que o grupo deve ser incluído</span><span class="sxs-lookup"><span data-stu-id="c0117-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="c0117-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0117-143">Response</span></span>
<span data-ttu-id="c0117-144">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0117-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0117-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0117-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0117-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0117-146">Request</span></span>
<span data-ttu-id="c0117-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0117-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="c0117-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0117-148">Response</span></span>
<span data-ttu-id="c0117-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0117-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```





