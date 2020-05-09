---
title: Criar deviceConfigurationAssignment
description: Criar um novo objeto deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f45636a129ad8a193ef0cdd2f2d73cf20dad611
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178665"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="3390b-103">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3390b-103">Create deviceConfigurationAssignment</span></span>

<span data-ttu-id="3390b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3390b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3390b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3390b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3390b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3390b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3390b-107">Criar um novo objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3390b-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3390b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3390b-108">Prerequisites</span></span>
<span data-ttu-id="3390b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3390b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3390b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3390b-111">Permission type</span></span>|<span data-ttu-id="3390b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3390b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3390b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3390b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3390b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3390b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3390b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3390b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3390b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3390b-116">Not supported.</span></span>|
|<span data-ttu-id="3390b-117">Application</span><span class="sxs-lookup"><span data-stu-id="3390b-117">Application</span></span>|<span data-ttu-id="3390b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3390b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3390b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3390b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3390b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3390b-120">Request headers</span></span>
|<span data-ttu-id="3390b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3390b-121">Header</span></span>|<span data-ttu-id="3390b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3390b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3390b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3390b-123">Authorization</span></span>|<span data-ttu-id="3390b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3390b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3390b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3390b-125">Accept</span></span>|<span data-ttu-id="3390b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3390b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3390b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3390b-127">Request body</span></span>
<span data-ttu-id="3390b-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="3390b-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="3390b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="3390b-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="3390b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3390b-130">Property</span></span>|<span data-ttu-id="3390b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3390b-131">Type</span></span>|<span data-ttu-id="3390b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3390b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3390b-133">id</span><span class="sxs-lookup"><span data-stu-id="3390b-133">id</span></span>|<span data-ttu-id="3390b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3390b-134">String</span></span>|<span data-ttu-id="3390b-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="3390b-135">The key of the assignment.</span></span>|
|<span data-ttu-id="3390b-136">destino</span><span class="sxs-lookup"><span data-stu-id="3390b-136">target</span></span>|[<span data-ttu-id="3390b-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3390b-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3390b-138">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3390b-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="3390b-139">source</span><span class="sxs-lookup"><span data-stu-id="3390b-139">source</span></span>|[<span data-ttu-id="3390b-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="3390b-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="3390b-141">A origem da atribuição para a configuração do dispositivo, direta ou de remessa/política.</span><span class="sxs-lookup"><span data-stu-id="3390b-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="3390b-142">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3390b-142">This property is read-only.</span></span> <span data-ttu-id="3390b-143">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="3390b-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="3390b-144">sourceId</span><span class="sxs-lookup"><span data-stu-id="3390b-144">sourceId</span></span>|<span data-ttu-id="3390b-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3390b-145">String</span></span>|<span data-ttu-id="3390b-146">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="3390b-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="3390b-147">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3390b-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="3390b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="3390b-148">Response</span></span>
<span data-ttu-id="3390b-149">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3390b-149">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3390b-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3390b-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="3390b-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3390b-151">Request</span></span>
<span data-ttu-id="3390b-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3390b-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="3390b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="3390b-153">Response</span></span>
<span data-ttu-id="3390b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3390b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 267

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



