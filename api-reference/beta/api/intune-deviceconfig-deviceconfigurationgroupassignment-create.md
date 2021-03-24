---
title: Criar deviceConfigurationGroupAssignment
description: Crie um novo objeto deviceConfigurationGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23cddf27e1622dcf6a661f8fcbbf24f49b436aba
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128072"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="dad0b-103">Criar deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="dad0b-103">Create deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="dad0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dad0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dad0b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dad0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dad0b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dad0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dad0b-107">Crie um novo [objeto deviceConfigurationGroupAssignment.](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="dad0b-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dad0b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dad0b-108">Prerequisites</span></span>
<span data-ttu-id="dad0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dad0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dad0b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dad0b-111">Permission type</span></span>|<span data-ttu-id="dad0b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dad0b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dad0b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dad0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dad0b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad0b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dad0b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dad0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dad0b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dad0b-116">Not supported.</span></span>|
|<span data-ttu-id="dad0b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dad0b-117">Application</span></span>|<span data-ttu-id="dad0b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad0b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dad0b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dad0b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="dad0b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dad0b-120">Request headers</span></span>
|<span data-ttu-id="dad0b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dad0b-121">Header</span></span>|<span data-ttu-id="dad0b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dad0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dad0b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dad0b-123">Authorization</span></span>|<span data-ttu-id="dad0b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dad0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dad0b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dad0b-125">Accept</span></span>|<span data-ttu-id="dad0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dad0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dad0b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dad0b-127">Request body</span></span>
<span data-ttu-id="dad0b-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="dad0b-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="dad0b-129">A tabela a seguir mostra as propriedades necessárias ao criar deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="dad0b-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="dad0b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dad0b-130">Property</span></span>|<span data-ttu-id="dad0b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dad0b-131">Type</span></span>|<span data-ttu-id="dad0b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dad0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dad0b-133">id</span><span class="sxs-lookup"><span data-stu-id="dad0b-133">id</span></span>|<span data-ttu-id="dad0b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dad0b-134">String</span></span>|<span data-ttu-id="dad0b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dad0b-135">Key of the entity.</span></span>|
|<span data-ttu-id="dad0b-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="dad0b-136">targetGroupId</span></span>|<span data-ttu-id="dad0b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dad0b-137">String</span></span>|<span data-ttu-id="dad0b-138">A ID do grupo AAD para o que estamos direcionando a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dad0b-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="dad0b-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="dad0b-139">excludeGroup</span></span>|<span data-ttu-id="dad0b-140">Booleano</span><span class="sxs-lookup"><span data-stu-id="dad0b-140">Boolean</span></span>|<span data-ttu-id="dad0b-141">Indica se esse grupo deve ser excluído.</span><span class="sxs-lookup"><span data-stu-id="dad0b-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="dad0b-142">Padrões de que o grupo deve ser incluído</span><span class="sxs-lookup"><span data-stu-id="dad0b-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="dad0b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="dad0b-143">Response</span></span>
<span data-ttu-id="dad0b-144">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dad0b-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dad0b-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dad0b-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="dad0b-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dad0b-146">Request</span></span>
<span data-ttu-id="dad0b-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dad0b-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dad0b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="dad0b-148">Response</span></span>
<span data-ttu-id="dad0b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dad0b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




