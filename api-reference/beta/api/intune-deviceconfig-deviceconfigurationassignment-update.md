---
title: Atualizar deviceConfigurationAssignment
description: Atualizar as propriedades de um objeto deviceConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c9b2c4a4a36b1d061a3b6bd47124b9455919888
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949459"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="e1daf-103">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e1daf-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="e1daf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1daf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1daf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1daf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1daf-106">Atualizar as propriedades de um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e1daf-106">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1daf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1daf-107">Prerequisites</span></span>
<span data-ttu-id="e1daf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1daf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1daf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1daf-110">Permission type</span></span>|<span data-ttu-id="e1daf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1daf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1daf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1daf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1daf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1daf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1daf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1daf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1daf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1daf-115">Not supported.</span></span>|
|<span data-ttu-id="e1daf-116">Application</span><span class="sxs-lookup"><span data-stu-id="e1daf-116">Application</span></span>|<span data-ttu-id="e1daf-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1daf-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1daf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1daf-118">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e1daf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1daf-119">Request headers</span></span>
|<span data-ttu-id="e1daf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1daf-120">Header</span></span>|<span data-ttu-id="e1daf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e1daf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1daf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1daf-122">Authorization</span></span>|<span data-ttu-id="e1daf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1daf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1daf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1daf-124">Accept</span></span>|<span data-ttu-id="e1daf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1daf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1daf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1daf-126">Request body</span></span>
<span data-ttu-id="e1daf-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e1daf-127">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="e1daf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e1daf-128">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="e1daf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1daf-129">Property</span></span>|<span data-ttu-id="e1daf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1daf-130">Type</span></span>|<span data-ttu-id="e1daf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1daf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1daf-132">id</span><span class="sxs-lookup"><span data-stu-id="e1daf-132">id</span></span>|<span data-ttu-id="e1daf-133">String</span><span class="sxs-lookup"><span data-stu-id="e1daf-133">String</span></span>|<span data-ttu-id="e1daf-134">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="e1daf-134">The key of the assignment.</span></span>|
|<span data-ttu-id="e1daf-135">destino</span><span class="sxs-lookup"><span data-stu-id="e1daf-135">target</span></span>|[<span data-ttu-id="e1daf-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e1daf-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e1daf-137">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e1daf-137">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="e1daf-138">source</span><span class="sxs-lookup"><span data-stu-id="e1daf-138">source</span></span>|[<span data-ttu-id="e1daf-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="e1daf-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="e1daf-140">A origem da atribuição para a configuração do dispositivo, direta ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="e1daf-140">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="e1daf-141">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1daf-141">This property is read-only.</span></span> <span data-ttu-id="e1daf-142">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="e1daf-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="e1daf-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="e1daf-143">sourceId</span></span>|<span data-ttu-id="e1daf-144">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e1daf-144">String</span></span>|<span data-ttu-id="e1daf-145">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="e1daf-145">The identifier of the source of the assignment.</span></span> <span data-ttu-id="e1daf-146">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1daf-146">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="e1daf-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1daf-147">Response</span></span>
<span data-ttu-id="e1daf-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1daf-148">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1daf-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1daf-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1daf-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1daf-150">Request</span></span>
<span data-ttu-id="e1daf-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1daf-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="e1daf-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1daf-152">Response</span></span>
<span data-ttu-id="e1daf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1daf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```





