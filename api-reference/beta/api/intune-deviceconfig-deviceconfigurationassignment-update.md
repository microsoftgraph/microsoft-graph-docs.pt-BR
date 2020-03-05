---
title: Atualizar deviceConfigurationAssignment
description: Atualizar as propriedades de um objeto deviceConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 41164d08e441e6be251a3f1f2b7637d07b632e07
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443094"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="59a23-103">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="59a23-103">Update deviceConfigurationAssignment</span></span>

<span data-ttu-id="59a23-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="59a23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59a23-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59a23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59a23-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59a23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59a23-107">Atualizar as propriedades de um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="59a23-107">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59a23-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59a23-108">Prerequisites</span></span>
<span data-ttu-id="59a23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59a23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59a23-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59a23-111">Permission type</span></span>|<span data-ttu-id="59a23-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59a23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59a23-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59a23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59a23-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59a23-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59a23-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59a23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59a23-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59a23-116">Not supported.</span></span>|
|<span data-ttu-id="59a23-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59a23-117">Application</span></span>|<span data-ttu-id="59a23-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59a23-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59a23-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59a23-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="59a23-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59a23-120">Request headers</span></span>
|<span data-ttu-id="59a23-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59a23-121">Header</span></span>|<span data-ttu-id="59a23-122">Valor</span><span class="sxs-lookup"><span data-stu-id="59a23-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59a23-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59a23-123">Authorization</span></span>|<span data-ttu-id="59a23-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59a23-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59a23-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="59a23-125">Accept</span></span>|<span data-ttu-id="59a23-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59a23-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59a23-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59a23-127">Request body</span></span>
<span data-ttu-id="59a23-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="59a23-128">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="59a23-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="59a23-129">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="59a23-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59a23-130">Property</span></span>|<span data-ttu-id="59a23-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="59a23-131">Type</span></span>|<span data-ttu-id="59a23-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="59a23-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59a23-133">id</span><span class="sxs-lookup"><span data-stu-id="59a23-133">id</span></span>|<span data-ttu-id="59a23-134">String</span><span class="sxs-lookup"><span data-stu-id="59a23-134">String</span></span>|<span data-ttu-id="59a23-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="59a23-135">The key of the assignment.</span></span>|
|<span data-ttu-id="59a23-136">destino</span><span class="sxs-lookup"><span data-stu-id="59a23-136">target</span></span>|[<span data-ttu-id="59a23-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="59a23-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="59a23-138">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59a23-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="59a23-139">source</span><span class="sxs-lookup"><span data-stu-id="59a23-139">source</span></span>|[<span data-ttu-id="59a23-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="59a23-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="59a23-141">A origem da atribuição para a configuração do dispositivo, direta ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="59a23-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="59a23-142">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59a23-142">This property is read-only.</span></span> <span data-ttu-id="59a23-143">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="59a23-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="59a23-144">sourceId</span><span class="sxs-lookup"><span data-stu-id="59a23-144">sourceId</span></span>|<span data-ttu-id="59a23-145">String</span><span class="sxs-lookup"><span data-stu-id="59a23-145">String</span></span>|<span data-ttu-id="59a23-146">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="59a23-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="59a23-147">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59a23-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="59a23-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="59a23-148">Response</span></span>
<span data-ttu-id="59a23-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59a23-149">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59a23-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59a23-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="59a23-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59a23-151">Request</span></span>
<span data-ttu-id="59a23-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59a23-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59a23-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="59a23-153">Response</span></span>
<span data-ttu-id="59a23-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59a23-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





