---
title: Criar deviceConfigurationGroupAssignment
description: Criar um novo objeto deviceConfigurationGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 66f0f1a2180e72ae2caad005157e4f75f5e4f81f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433404"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="fea6e-103">Criar deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="fea6e-103">Create deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="fea6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fea6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fea6e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fea6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fea6e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fea6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fea6e-107">Criar um novo objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fea6e-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fea6e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fea6e-108">Prerequisites</span></span>
<span data-ttu-id="fea6e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fea6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fea6e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fea6e-111">Permission type</span></span>|<span data-ttu-id="fea6e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fea6e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fea6e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fea6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fea6e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fea6e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fea6e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fea6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fea6e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fea6e-116">Not supported.</span></span>|
|<span data-ttu-id="fea6e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fea6e-117">Application</span></span>|<span data-ttu-id="fea6e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fea6e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fea6e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fea6e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="fea6e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fea6e-120">Request headers</span></span>
|<span data-ttu-id="fea6e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fea6e-121">Header</span></span>|<span data-ttu-id="fea6e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fea6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fea6e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fea6e-123">Authorization</span></span>|<span data-ttu-id="fea6e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fea6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fea6e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fea6e-125">Accept</span></span>|<span data-ttu-id="fea6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fea6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fea6e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fea6e-127">Request body</span></span>
<span data-ttu-id="fea6e-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="fea6e-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="fea6e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="fea6e-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="fea6e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fea6e-130">Property</span></span>|<span data-ttu-id="fea6e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fea6e-131">Type</span></span>|<span data-ttu-id="fea6e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fea6e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fea6e-133">id</span><span class="sxs-lookup"><span data-stu-id="fea6e-133">id</span></span>|<span data-ttu-id="fea6e-134">String</span><span class="sxs-lookup"><span data-stu-id="fea6e-134">String</span></span>|<span data-ttu-id="fea6e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fea6e-135">Key of the entity.</span></span>|
|<span data-ttu-id="fea6e-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="fea6e-136">targetGroupId</span></span>|<span data-ttu-id="fea6e-137">String</span><span class="sxs-lookup"><span data-stu-id="fea6e-137">String</span></span>|<span data-ttu-id="fea6e-138">A ID do grupo do AAD no qual estamos direcionando a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fea6e-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="fea6e-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="fea6e-139">excludeGroup</span></span>|<span data-ttu-id="fea6e-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="fea6e-140">Boolean</span></span>|<span data-ttu-id="fea6e-141">Indica se esse grupo deve ser excluído.</span><span class="sxs-lookup"><span data-stu-id="fea6e-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="fea6e-142">Padrões que o grupo deve ser incluído</span><span class="sxs-lookup"><span data-stu-id="fea6e-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="fea6e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea6e-143">Response</span></span>
<span data-ttu-id="fea6e-144">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fea6e-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fea6e-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fea6e-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="fea6e-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fea6e-146">Request</span></span>
<span data-ttu-id="fea6e-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fea6e-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fea6e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea6e-148">Response</span></span>
<span data-ttu-id="fea6e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fea6e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



