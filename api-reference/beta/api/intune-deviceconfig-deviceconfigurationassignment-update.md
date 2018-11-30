---
title: Atualizar deviceConfigurationAssignment
description: Atualizar as propriedades de um objeto deviceConfigurationAssignment.
ms.openlocfilehash: 2933f66f648a00f4fd66dd4ec20cbcbba395acd2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035830"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="e02f9-103">Atualizar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e02f9-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="e02f9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e02f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e02f9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e02f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e02f9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e02f9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e02f9-107">Atualizar as propriedades de um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e02f9-107">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e02f9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e02f9-108">Prerequisites</span></span>
<span data-ttu-id="e02f9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e02f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e02f9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e02f9-111">Permission type</span></span>|<span data-ttu-id="e02f9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e02f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e02f9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e02f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e02f9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e02f9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e02f9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e02f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e02f9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e02f9-116">Not supported.</span></span>|
|<span data-ttu-id="e02f9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e02f9-117">Application</span></span>|<span data-ttu-id="e02f9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e02f9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e02f9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e02f9-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e02f9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e02f9-120">Request headers</span></span>
|<span data-ttu-id="e02f9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e02f9-121">Header</span></span>|<span data-ttu-id="e02f9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e02f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e02f9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e02f9-123">Authorization</span></span>|<span data-ttu-id="e02f9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e02f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e02f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e02f9-125">Accept</span></span>|<span data-ttu-id="e02f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e02f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e02f9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e02f9-127">Request body</span></span>
<span data-ttu-id="e02f9-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e02f9-128">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="e02f9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e02f9-129">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="e02f9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e02f9-130">Property</span></span>|<span data-ttu-id="e02f9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e02f9-131">Type</span></span>|<span data-ttu-id="e02f9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e02f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e02f9-133">id</span><span class="sxs-lookup"><span data-stu-id="e02f9-133">id</span></span>|<span data-ttu-id="e02f9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e02f9-134">String</span></span>|<span data-ttu-id="e02f9-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="e02f9-135">The key of the assignment.</span></span>|
|<span data-ttu-id="e02f9-136">destino</span><span class="sxs-lookup"><span data-stu-id="e02f9-136">target</span></span>|[<span data-ttu-id="e02f9-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e02f9-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e02f9-138">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e02f9-138">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="e02f9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e02f9-139">Response</span></span>
<span data-ttu-id="e02f9-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e02f9-140">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e02f9-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e02f9-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="e02f9-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e02f9-142">Request</span></span>
<span data-ttu-id="e02f9-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e02f9-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e02f9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e02f9-144">Response</span></span>
<span data-ttu-id="e02f9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e02f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





