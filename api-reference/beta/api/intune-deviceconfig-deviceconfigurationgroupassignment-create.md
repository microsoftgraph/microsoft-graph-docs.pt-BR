---
title: Criar deviceConfigurationGroupAssignment
description: Criar um novo objeto deviceConfigurationGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00da2479c36d9b9780264e19d48a838b4ab838eb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949354"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="2c21e-103">Criar deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="2c21e-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="2c21e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c21e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c21e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c21e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c21e-106">Criar um novo objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2c21e-106">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c21e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2c21e-107">Prerequisites</span></span>
<span data-ttu-id="2c21e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c21e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c21e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c21e-110">Permission type</span></span>|<span data-ttu-id="2c21e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2c21e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c21e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c21e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c21e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c21e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c21e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c21e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c21e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c21e-115">Not supported.</span></span>|
|<span data-ttu-id="2c21e-116">Application</span><span class="sxs-lookup"><span data-stu-id="2c21e-116">Application</span></span>|<span data-ttu-id="2c21e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c21e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c21e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c21e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="2c21e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c21e-119">Request headers</span></span>
|<span data-ttu-id="2c21e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c21e-120">Header</span></span>|<span data-ttu-id="2c21e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2c21e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c21e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c21e-122">Authorization</span></span>|<span data-ttu-id="2c21e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c21e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c21e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2c21e-124">Accept</span></span>|<span data-ttu-id="2c21e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c21e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c21e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c21e-126">Request body</span></span>
<span data-ttu-id="2c21e-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="2c21e-127">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="2c21e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="2c21e-128">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="2c21e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c21e-129">Property</span></span>|<span data-ttu-id="2c21e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c21e-130">Type</span></span>|<span data-ttu-id="2c21e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c21e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c21e-132">id</span><span class="sxs-lookup"><span data-stu-id="2c21e-132">id</span></span>|<span data-ttu-id="2c21e-133">String</span><span class="sxs-lookup"><span data-stu-id="2c21e-133">String</span></span>|<span data-ttu-id="2c21e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2c21e-134">Key of the entity.</span></span>|
|<span data-ttu-id="2c21e-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="2c21e-135">targetGroupId</span></span>|<span data-ttu-id="2c21e-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2c21e-136">String</span></span>|<span data-ttu-id="2c21e-137">A ID do grupo do AAD no qual estamos direcionando a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c21e-137">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="2c21e-138">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="2c21e-138">excludeGroup</span></span>|<span data-ttu-id="2c21e-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c21e-139">Boolean</span></span>|<span data-ttu-id="2c21e-140">Indica se esse grupo deve ser excluído.</span><span class="sxs-lookup"><span data-stu-id="2c21e-140">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="2c21e-141">Padrões que o grupo deve ser incluído</span><span class="sxs-lookup"><span data-stu-id="2c21e-141">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="2c21e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c21e-142">Response</span></span>
<span data-ttu-id="2c21e-143">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c21e-143">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c21e-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c21e-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c21e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c21e-145">Request</span></span>
<span data-ttu-id="2c21e-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c21e-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="2c21e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c21e-147">Response</span></span>
<span data-ttu-id="2c21e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c21e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```





